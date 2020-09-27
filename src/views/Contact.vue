<template>
    <div class="contact">
        <Email />
    </div>
</template>

<script>
import Email from '../components/Email'
export default {
    components: {Email}
}
</script>


<style>
.contact {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    /* position: absolute; */
    bottom: 300px
}

@media (min-width: 768px) and (max-width: 1024px) {
    .contact {
        bottom: 700px;
        padding: 20px;
        /* width: 90%; */
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .contact {
        bottom: 700px;
        padding: 20px;
        /* width: 90%; */
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .contact {
        bottom: 700px;
        padding: 20px;
        /* width: 90%; */
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .contact {
        bottom: 700px;
        padding: 20px;
        /* width: 90%; */
    }
}
</style>
