<script setup>
import {ref} from "vue";
import { useRouter } from "vue-router";

const router=useRouter();
const email=ref("");
const password=ref("");
const inputCtnBorderAlertStyle=ref('1px solid #3C2708');

const submitLoginDetails=()=>{
    if (((email.value==="") || (password.value===""))||((email.value==="") && (password.value===""))){
        inputCtnBorderAlertStyle.value="1px solid red";
    }
    else{
        router.push('/home')
    }
}
</script>

<template>
    <div   
        class="auth-login-main-ctn"
    >
        <h2 
            class="auth-login-main-ctn-title"
        >
            Login
        </h2>
        <br/>
        <form 
            action="" 
            class="auth-login-main-ctn-form" 
            @submit.prevent="submitLoginDetails"
        >
            <div 
                class="auth-login-main-ctn-form-input-and-label-ctn"
            >
                <label 
                    for="email" 
                    class="auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name"
                >
                    Email
                </label>
                <input 
                    v-model="email" 
                    id="email" 
                    type="email" 
                    :style="{borderBottom: inputCtnBorderAlertStyle}" 
                />
            </div>
            <br/>
            <div 
                class="auth-login-main-ctn-form-input-and-label-ctn">
                <label 
                    for="password" 
                    class="auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name"
                >
                    Password
                </label>
                <input 
                    v-model="password" 
                    id="password" 
                    type="password" 
                    :style="{borderBottom: inputCtnBorderAlertStyle}" 
                />
            </div>
            <br/>
            <button @click="submitLoginDetails" type="submit" class="auth-login-main-ctn-form-input-and-label-ctn-submit-btn">
                Login
            </button>
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
    text-transform: capitalize;
}
.auth-login-main-ctn-form-input-and-label-ctn input{
    background-color: transparent;
    width:100%;
    padding:5px 10px;
    font-size:16px;
    border: 0;
}
.auth-login-main-ctn-form-input-and-label-ctn-submit-btn{
    width: 100%;
    padding: 10px 16px;
    background-color: #3C2708;
    color: #fff;
    font-size: 18px;
}
.auth-login-main-ctn-form-input-and-label-ctn-submit-btn:hover{
    cursor: pointer;
    background-color: transparent;
    color:#3C2708;
    border: 1px solid #3C2708;
    transform: scale(0.98);
    transition: all .4s;
}

@media screen and (max-width: 900px) {
    .auth-login-main-ctn-title{
        font-size: 22px;
    }
    .auth-login-main-ctn-form-input-and-label-ctn-input-ctn-name{
        font-size: 12px;
    }
    .auth-login-main-ctn-form-input-and-label-ctn input{
        font-size: 14px;
        padding: 0 5px;
    }
    .auth-login-main-ctn-form-input-and-label-ctn-submit-btn{
        padding: 5px 8px;
        font-size: 16px;
    }
}
</style>