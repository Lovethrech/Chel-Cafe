<script setup>
import AuthSignUpType from './AuthSignUpType.vue';
</script>

<template>
    <div class="auth-signup-main-ctn">
        <h3 class="auth-signup-main-ctn-title">
            or sign up using
        </h3>
        <div class="auth-signup-mini-ctn">
            <AuthSignUpType></AuthSignUpType>
        </div>
        <div class="auth-signup-main-ctn-email-type-ctn">
            <p class="auth-signup-main-ctn-email-type-ctn-desc">
                sign up with email
            </p>
        </div>
    </div>
</template>

<style scoped>
.auth-signup-main-ctn{
    text-align: center;
}
.auth-signup-main-ctn-title{
    text-transform: capitalize;
}
</style>