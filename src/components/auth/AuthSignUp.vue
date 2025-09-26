<script setup>
import authSignUpDetails from '@/data/authSignUpDetails.json';
import AuthSignUpType from './AuthSignUpType.vue';
</script>

<template>
    <div 
        class="auth-signup-main-ctn"
    >
        <h3 
            class="auth-signup-main-ctn-title"
        >
            or sign up using
        </h3>
        <br/>
        <div 
            class="auth-signup-mini-ctn">
            <AuthSignUpType
                v-for="authSignUpDetail in authSignUpDetails"
                :key="authSignUpDetail.id"
                :name="authSignUpDetail.name"
                :src="authSignUpDetail.src"
                :link="authSignUpDetail.link"
            >
            </AuthSignUpType>
        </div>
        <br/>
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
.auth-signup-main-ctn-title, .auth-signup-main-ctn-email-type-ctn-desc{
    text-transform: capitalize;
}
.auth-signup-main-ctn-title{
    color:#a3a3a3;
    font-size: 14px;
}
.auth-signup-mini-ctn{
    display:flex;
    justify-content: center;
    place-items: center;
    gap:14px;
}
.auth-signup-main-ctn-email-type-ctn-desc{
    color:#000000;
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