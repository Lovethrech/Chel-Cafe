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
                :imgSrc="imgSrc"
                :name="name"
            >
            </HomeOfferImg>
            <HomeOfferBtn
                :link="link"
            >
            </HomeOfferBtn>
        </div>
    </div>
</template>

<style scoped>
#home-offer-main-ctn{
    margin: 10px 0;
    display: flex;
    justify-content: center;
    place-items: center;
    background-color: red;
    width: 40%;
    min-height: 30vh;
}
</style>