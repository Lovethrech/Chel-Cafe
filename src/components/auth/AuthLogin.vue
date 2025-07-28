<script setup>
import {ref} from "vue";

const inputCtnBorderAlertStyle=ref('3px solid red');
</script>

<template>
    <div class="auth-login-main-ctn">
        <h2 class="auth-login-main-ctn-title">
            Login
        </h2>
        <br/>
        <form action="" class="auth-login-main-ctn-form">
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                <input v-model="email" id="" type="" :style="{borderBottom: inputCtnBorderAlertStyle}" required/>
                <label for="" class="auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name">Username</label>
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