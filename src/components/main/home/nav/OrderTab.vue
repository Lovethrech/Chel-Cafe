<template>
    <div 
        class="main-home-nav-order-tab-main-ctn"
    >
        <RouterLink 
            to="/orders" 
            class="link"
        >
            <p 
                class="main-home-nav-order-tab-main-ctn-desc"
            >
                Orders
            </p>
        </RouterLink>    
    </div>
</template>

<style scoped>
.main-home-nav-order-tab-main-ctn{
    background-color: lavender;
    margin: 0 4vh 1vh;
    width: 100%;
    display:flex;
    justify-content: right;
}
.link{
    margin:inherit;
}
.main-home-nav-order-tab-main-ctn-desc{
    margin-right: 3vw;
    padding: 1vh 10;
    background-color: #3C2708;
    color:#fff;
    font-size: 12px;
    border-radius: 20px;
    border: 1px solid #3C2708;
}
.main-home-nav-order-tab-main-ctn-desc:hover{
    cursor: pointer;
    background-color: transparent;
    color: #3C2708;
    border: 1px solid #3C2708;
    transform: scale(0.98);
    transition: all .4s;
}

@media screen and (max-width: 440px) {
    .main-home-nav-order-tab-main-ctn-desc{
        font-size: 10px;
    }
}
</style>