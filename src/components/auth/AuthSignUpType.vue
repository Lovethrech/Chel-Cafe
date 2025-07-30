<script setup>
import { defineProps } from 'vue';

const {name, link}=defineProps(['name', 'link']);
</script>

<template>
    <a href="" class="auth-sign-up-type-main-ctn-link">
        <div class="auth-sign-up-type-main-ctn">
            <img :src="@/components/Icons/apple.svg" alt="">
        </div>
    </a>
</template>

<style scoped>
.auth-sign-up-type-main-ctn{
    width:30px;
}
.auth-sign-up-type-main-ctn img{
    width:100%;
    height:100%;
}
</style>