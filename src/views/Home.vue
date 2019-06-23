<template>
    <div class="home">
        <div data-aos="zoom-in" id="home-img-intro"><img class="responsive-img" src="../assets/images/illustration-intro.png" alt="fylo home image"></div>
        <div id="home-text-intro">
            <span class="white size-35">
                All your files in one secure location, <br/>
                accesible anywhere
            </span>
        </div>
        <div id="home-extra-text-intro">
            <span class="white">
                Fylo stores all your most important files in one secure location.
                Access them wherever you need, share and collaborate with friends, family and co-workers.
            </span>
        </div>
        <div class="getting-started-wrapper">
            <Button>
                Get Started
            </Button>
        </div>
    </div>
</template>

<script>
import Button from '../components/Button';
export default {
    components: {
        Button
    }
}
</script>


<style scoped>
 * { text-align: center}

.home {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.getting-started-wrapper {
    padding-top: 40px;
}

#home-text-intro {
    font-weight: 700;
    padding: 35px 0 35px 0
}

#home-extra-text-intro {
    width: 50%;
    font-weight: 400;
}

@media (min-width: 768px) and (max-width: 1024px) {
    #home-img-intro {
        padding: 0 20px 0 20px
    }

    #home-extra-text-intro {
        width: 100%;
        padding: 0 40px 0 40px;
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    #home-img-intro {
        padding: 0 20px 0 20px
    }

    #home-extra-text-intro {
        width: 100%;
        padding: 0 40px 0 40px;
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    #home-img-intro {
        padding: 0 20px 0 20px
    }

    #home-extra-text-intro {
        width: 100%;
        padding: 0 40px 0 40px;
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    #home-img-intro {
        padding: 0 20px 0 20px
    }

    #home-extra-text-intro {
        width: 100%;
        padding: 0 40px 0 40px;
    }
}

</style>

