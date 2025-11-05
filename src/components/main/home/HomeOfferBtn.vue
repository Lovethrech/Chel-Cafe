<script setup>
import { defineProps } from 'vue';

const {link}= defineProps(['link']);
</script>

<template>
    <div 
        class="home-offer-btn-main-ctn"
    >
        <RouterLink 
            :to="link"
        >
            <button 
                class="home-offer-main-btn"
            >
                View offers
            </button>
        </RouterLink>
    </div>
</template>

<style scoped>
.home-offer-btn-main-ctn{
    
    margin-bottom: -10px;
    background-color: #1289;
}
</style>