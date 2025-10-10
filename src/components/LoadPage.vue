<script setup>
import LoadPageText from './LoadPageText.vue';
</script>

<template>
    <div 
        class="load-page-main-ctn"
    >
        <div 
            class="load-page-mini-ctn">
            <LoadPageText></LoadPageText>
        </div>
    </div>
</template>

<style scoped>
.load-page-main-ctn{
    width:100%;
    height: 100vh;
    background:  url(/LoadPageTopLeaf.png) top right / 100px no-repeat, 
        url(/LoadPageBottomLeaf.png) bottom left / 100px no-repeat ;
    display:flex;
    justify-content: center;
    place-items: center;
}
</style>
