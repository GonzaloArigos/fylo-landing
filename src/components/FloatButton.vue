<template>
    <button v-scroll-to="'.home'" class="float-btn">
        <span class="bold white" id="arrow-float-btn">⌃</span>  
    </button>    
</template>

<style scoped>
.float-btn {
    z-index: 100;
    width: 50px;
    height: 50px;
    cursor: pointer;
    border-radius: 50%;
    background-color: #44b2d0;
    color: white;
    position: fixed;
    bottom: 30px;
    right: 30px;
    outline: none;
    border: none;
    transition: all ease-in-out 300ms;
    padding-top: 15px
}

.float-btn:hover {
  transform: translate(0px, -10px);
}

#arrow-float-btn {
    font-size: 30px;
}

@media (min-width: 768px) and (max-width: 1024px) {
    .float-btn {
        right: 30px;
        padding-top: 10px
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .float-btn {
        right: 30px;
        padding-top: 10px
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .float-btn {
        right: 30px;
        padding-top: 10px
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .float-btn {
        right: 30px;
        padding-top: 10px
    }
}
</style>


