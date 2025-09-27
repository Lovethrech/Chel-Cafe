<script setup>
import { defineProps } from 'vue';

import HomeOfferImg from './HomeOfferImg.vue';
import HomeOfferBtn from './HomeOfferBtn.vue';

const {name, imgSrc, link}=defineProps(['name', 'imgSrc', 'link']);
</script>

<template>
    <div 
        id="home-offer-main-ctn"
    >
        <div 
            id="home-offer-mini-ctn"
        >
            <HomeOfferImg

            >
            </HomeOfferImg>
            <HomeOfferBtn
            
            >
            </HomeOfferBtn>
        </div>
    </div>
</template>

<style scoped>
#home-offer-main-ctn{
    display: flex;
    justify-content: center;
    place-items: center;
}
</style>