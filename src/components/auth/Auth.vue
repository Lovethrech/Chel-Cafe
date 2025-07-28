<script setup>
import AuthLogin from './AuthLogin.vue';
</script>

<template>
    <div class="auth-main-ctn">
        <div class="auth-mini-ctn">
            <AuthLogin></AuthLogin>
        </div>
    </div>
</template>

<style scoped>
.auth-main-ctn{
    width:100%;
    height: 100vh;
    background:  url(/LoadPageTopLeaf.png) top right / 100px no-repeat, 
        url(/LoadPageBottomLeaf.png) bottom left / 100px no-repeat ;
    display:flex;
    justify-content: center;
    place-items: center;
}
.auth-mini-ctn{
    background-color: #f0eeee;
    width:50%;
    height:50%;
    padding:3vh 4vw;
}

@media screen and (max-width: 900px) {
    .auth-mini-ctn{
        width:80%;
        height:66%;
    }
}
</style>