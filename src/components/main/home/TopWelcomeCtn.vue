<script setup>
import OrderTab from './nav/OrderTab.vue';
</script>

<template>
    <div 
        class="main-top-welcome-ctn-main-ctn"
    >
        <div 
            class="main-top-welcome-ctn-mini-ctn"
        >
            <h2 
                class="main-top-welcome-ctn-mini-ctn-title">
                Welcome to Chel Brewhouse 
            </h2>
        </div>
        <OrderTab></OrderTab>
    </div>
</template>

<style scoped>
.main-top-welcome-ctn-main-ctn{
    display: flex;
    flex-direction: column;
    justify-content: left;
    place-items: center;
    width:100%;
    background:  url(/LoadPageTopLeaf.png) #F7E7CE top right / 60px no-repeat;
    color: #3C2708;
}
.main-top-welcome-ctn-mini-ctn{
    width: inherit;
    padding:10px 90px 10px 40px;
}
.main-top-welcome-ctn-mini-ctn-title{
    text-align: left;
    font-size: 36px;
}

@media screen and (max-width: 440px) {
    .main-top-welcome-ctn-main-ctn{
        background:  url(/LoadPageTopLeaf.png) #F7E7CE top right / 50px no-repeat;
    }
    .main-top-welcome-ctn-mini-ctn{
        padding:5px 90px 5px 40px;
    }
    .main-top-welcome-ctn-mini-ctn-title{
        font-size: 26px;
    }
}
</style>