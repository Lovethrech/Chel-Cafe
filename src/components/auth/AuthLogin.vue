<script setup>
import {ref} from "vue";

const inputCtnBorderAlertStyle=ref('1px solid hsl(36, 76%, 13%)');
const namePositionPlacement=ref("50%");

</script>

<template>
    <div class="auth-login-main-ctn">
        <h2 class="auth-login-main-ctn-title">
            Login
        </h2>
        <br/>
        <form action="" class="auth-login-main-ctn-form">
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                <input 
                    v-model="email" 
                    id="email" 
                    type="email" 
                    :style="{borderBottom: inputCtnBorderAlertStyle}" 
                    required
                />
                <label 
                    for="email" 
                    class="auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name"
                >
                    Username
                </label>
            </div>
            <br/>
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                <input 
                    v-model="password" 
                    id="password" 
                    type="password" 
                    :style="{borderBottom: inputCtnBorderAlertStyle}" 
                    required
                />
                <label 
                    for="password" 
                    class="auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name"
                >
                    Password
                </label>
            </div>
        </form>
    </div>
</template>
<style scoped>
.auth-login-main-ctn-title{
    text-transform: uppercase;
    text-align: center;
    color: hsl(36, 76%, 13%);
    font-family: "Michroma", sans-serif;
    font-size:34px;
    font-weight: 600;
}
.auth-login-main-ctn-form-input-and-label-ctn{
    display:flex;
    flex-direction: column;
}
.auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name{
    position:absolute;
    font-size:2vh;
    color:rgb(0, 0, 0);
    font-weight:400;
    transform: translateY(-50%);
    transition: all .5s;
}
.auth-login-main-ctn-form-input-and-label-ctn input{
    background: transparent;
    color:transparent;
    margin-right:0;
    width:100%;
    height:100%;
    outline:0;
    border:0;
    font-size:2vh;
    padding: 2px 10px;
}
</style>