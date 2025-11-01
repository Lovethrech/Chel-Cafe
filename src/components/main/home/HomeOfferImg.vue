<script setup>
import { defineProps } from 'vue';

const {name, imgSrc}= defineProps(['name', 'imgSrc']);

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
    width: 100%;
    height: 100%;
}
</style>