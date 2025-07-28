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
            <a href="" class="auth-signup-main-ctn-email-type-ctn-link">
                <p class="auth-signup-main-ctn-email-type-ctn-desc">
                    sign up with email
                </p>
            </a>
        </div>
    </div>
</template>

<style scoped>
.auth-signup-main-ctn{
    text-align: center;
}
.auth-signup-main-ctn-title{
    color:#a3a3a3;
    text-transform: capitalize;
    font-size: 14px;
}
.auth-signup-main-ctn-email-type-ctn-desc{
    color:#000000;
    text-transform: capitalize;
    text-decoration-line: underline;
    font-size: 20px;
}

@media screen and (max-width: 900px) {
    .auth-signup-main-ctn-title{
        font-size: 12px;
    }
    .auth-signup-main-ctn-email-type-ctn-desc{
        font-size: 16px;
    }
}
</style>