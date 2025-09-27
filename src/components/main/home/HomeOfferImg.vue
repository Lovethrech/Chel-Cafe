<script setup>
import { defineProps } from 'vue';

const {name, imgSrc}= defineProps(['name', 'imgSrc']);
// plan to work on side nav with respect to mobile bottom nav 
</script>

<template>
    <div class="home-offer-img-ctn">
        <img 
            :src="imgSrc" 
            :alt="name" 
            width="100%"
            height="100%"
        />
    </div>
</template>

<style scoped>
.home-offer-img-ctn{
    background-color: #fff;
    width:700px;
}
</style>