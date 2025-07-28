<script setup>
import {ref} from "vue";

const inputCtnBorderAlertStyle=ref('1px solid #3C2708');
</script>

<template>
    <div class="auth-login-main-ctn">
        <h2 class="auth-login-main-ctn-title">
            Login
        </h2>
        <br/>
        <form action="" class="auth-login-main-ctn-form">
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                <label 
                    for="" 
                    class="auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name"
                >
                    Username
                </label>
                <input 
                    v-model="email" 
                    id="" 
                    type="" 
                    :style="{borderBottom: inputCtnBorderAlertStyle}" 
                    required
                />
            </div>
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                
            </div>
        </form>
    </div>
</template>
<style scoped>
.auth-login-main-ctn-title{
    text-transform: uppercase;
    text-align: center;
    color: #3C2708;
    font-family: "Michroma", sans-serif;
    font-size:34px;
    font-weight: 600;
}
.auth-login-main-ctn-form-input-and-label-ctn{
    display:flex;
    flex-direction: column;
}
.auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name{
    color:#6a6a6a;
    font-size:14px;
    font-weight: 400;
    letter-spacing: 0.25px;
    text-transform: capitalize;
}
.auth-login-main-ctn-form-input-and-label-ctn input{
    background-color: transparent;
    width:100%;
    height:40px;
    padding:4px;
    font-size:20px;
    border: 0;
}
</style>