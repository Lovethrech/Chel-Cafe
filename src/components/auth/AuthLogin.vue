<script setup>
import {ref} from "vue";

const inputCtnBorderAlertStyle=ref('3px solid #ededed');
</script>

<template>
    <div class="auth-login-main-ctn">
        <form action="" class="auth-login-main-ctn-form">
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                <label for="" class="input-ctn-name">Username</label>
                <input v-model="email" id="" type="" :style="{border: inputCtnBorderAlertStyle}" required/>
                
            </div>
            <div class="auth-login-main-ctn-form-input-and-label-ctn">
                
            </div>
        </form>
    </div>
</template>