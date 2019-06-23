<template>
    <button class="btn-blue white">
        <slot></slot>
    </button>    
</template>

<style>
.btn-blue {
    background-color: #44b2d0;
    font-weight: 700;
    border-radius: 100px;
    padding: 15px 40px 15px 40px;
    cursor: pointer;
    border: none;
    outline: none;
    font-size: 15px;
    transition: all 0.3s
}

.btn-blue:hover {
    transform: scale(1.04);
    -webkit-box-shadow: -1px 0px 21px -10px rgba(0,0,0,0.45);
    -moz-box-shadow: -1px 0px 21px -10px rgba(0,0,0,0.45);
    box-shadow: -1px 0px 21px -10px rgba(0,0,0,0.45);
}

@media (min-width: 768px) and (max-width: 1024px) {
    .btn-blue {
        width: 100%
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .btn-blue {
        width: 100%
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .btn-blue {
        width: 100%
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .btn-blue {
        width: 100%
    }
}

</style>

