<template>
<div class="mt-5">
   <h2 class="text-white text-center">Nosotros</h2>
    <div class="reviews mb-3 mt-2">
    
        <div data-aos="flip-left" v-for="(review, i) in reviews" :key="i">
           
            <ReviewCard 
                :avatar="review.avatar"
                :name="review.name"
                :position="review.position"
                :review="review.review"
            />
        </div>
    </div>
    </div>
</template>

<script>
import ReviewCard from '../components/ReviewCard';
import data from '../data';

export default {
    components: {
        ReviewCard
    },

    data() {
        return {
            reviews: []
        }
    },
    beforeMount() {
        this.reviews = data;
    }
}    

</script>

<style>
.reviews {
    display: flex;
    justify-content: space-between;
    padding: 80px 100px 280px 100px;
}

@media (min-width: 768px) and (max-width: 1024px) {
    .reviews {
        padding: 0;
        flex-direction: column;
        align-items: center;
    }

    .reviews > div {
        padding-top: 40px;
    }

}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .reviews {
        padding: 0;
        flex-direction: column;
        align-items: center;
    }

    .reviews > div {
        padding-top: 40px;
    }

}

@media (min-width: 481px) and (max-width: 767px) {
    .reviews {
        padding: 0;
        flex-direction: column;
        align-items: center;
    }

    .reviews > div {
        padding-top: 40px;
    }

}

@media (min-width: 320px) and (max-width: 480px) {
    .reviews {
        padding: 0;
        flex-direction: column;
        align-items: center;
    }

    .reviews > div {
        padding-top: 40px;
    }

}
</style>


