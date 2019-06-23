<template>
    <div class="header">
        <div id="logo-wrapper">
            <img src="../assets/images/logo.svg" alt="" class="logo-img">
        </div>
        <div class="header-items">
            <div class="mobile-menu-icon"><span><i class="fa fa-bars"></i></span></div>
            <div class="web-item"><span v-scroll-to="'.services'">Services</span></div>
            <div class="web-item"><span v-scroll-to="'.offer'">Productive</span></div>
            <div class="web-item"><span v-scroll-to="'.reviews'">Reviews</span></div>
        </div>
    </div>
</template>

<style>
.header {
    flex: 1;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 50px 20px 50px
}
.header-items {
    width: 30%;
    display: flex;
    justify-content: space-between
}
.mobile-menu-icon {
    display: none;
}
.header-items > div {
    color: white;
    cursor: pointer;
    transition: all 0.5s;
}
.header-items > div:hover {
    color: rgba(241, 241, 241, 0.582)
}

@media (min-width: 768px) and (max-width: 1024px) {
    .logo-img {
        width: 100px;
    }
    .web-item {
        display: none;
        /* width: 60%;
        align-items: center */
    }
    .mobile-menu-icon {
        display: block;
    
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .header {
        padding: 20px;
    }
    .logo-img {
        width: 100px;
    }
    .web-item {
        display: none;
        /* width: 60%;
        align-items: center */
    }
    .mobile-menu-icon {
        display: block;
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .header {
        padding: 20px;
    }
    .logo-img {
        width: 100px;
    }
    .web-item {
        display: none;
        /* width: 60%;
        align-items: center */
    }
    .mobile-menu-icon {
        display: block;
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .header {
        padding: 20px;
    }
    .logo-img {
        width: 100px;
    }
    .web-item {
        display: none;
        /* width: 60%;
        align-items: center */
    }
    .mobile-menu-icon {
        display: block;
    }
}
</style>
