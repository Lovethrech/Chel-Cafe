<script setup>
import {ref} from "vue";

const inputCtnBorderAlertStyle=ref('3px solid #ededed');
</script>

<template>
    <div class="auth-login-main-ctn">
        <h2 class="auth-login-main-ctn-title">
            Login
        </h2>
        <form action="" class="auth-login-main-ctn-form">
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                <label for="" class="auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name">Username</label>
                <input v-model="email" id="" type="" :style="{border: inputCtnBorderAlertStyle}" required/>
                
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
</style>