<script setup>
import { defineProps } from 'vue';

const {name, src, link}=defineProps(['name', 'src', 'link']);
</script>

<template>
    <a 
        :href="link" 
        class="auth-sign-up-type-main-ctn-link"
    >
        <div 
            class="auth-sign-up-type-main-ctn"
        >
            <img 
                :src="src" 
                :alt="name">
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