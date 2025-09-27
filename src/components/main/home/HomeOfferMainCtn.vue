<script setup>
import HomeOfferDetails from "@/data/home-offer-details.json";
import HomeOffer from './HomeOffer.vue';
</script>

<template>
    <section id="home-offer-main-ctn-main-ctn">
        <div id="home-offer-main-ctn-mini-ctn">
            <HomeOffer></HomeOffer>
        </div>
    </section>
</template>

<style scoped>
#home-offer-main-ctn-main-ctn{
    padding:2vh 4vw;
    width: 100%;
    min-height:90vh;
    background-color: #234523;
}
#home-offer-main-ctn-mini-ctn{
    width: 100%;
    height: 100%;
    background-color: #122812;
}
</style>