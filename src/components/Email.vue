<template>
    <div data-aos="zoom-in" class="email">
        <div>
            <span class="bold white size-35 email-title">Get early access today</span>
        </div> <br>
        <div>
            <span class="white">It only takes a minute to sign up and our free starter tier is extremely generous. If you have any questions, our support team would be happy to help you</span>
        </div> <br>
        <div class="inputAndButton">
            <div id="input-wrapper">
                <input placeholder="email@test.com" type="text" id="email-input">
            </div>
            <div id="button-wrapper">
                <Button>
                    Get Started For Free
                </Button>
            </div>
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


<style>
.email {
    display: flex;
    width: 50%;
    border-radius: 5px;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    padding: 40px;
    align-items: center;
    background: hsl(217, 28%, 15%);
    cursor: pointer;
    -webkit-box-shadow: -1px 3px 5px 0px rgba(0,0,0,0.39);
    -moz-box-shadow: -1px 3px 5px 0px rgba(0,0,0,0.39);
    box-shadow: -1px 3px 5px 0px rgba(0,0,0,0.39);    
}

.inputAndButton {
    width: 100%;
    display: flex;
}

#input-wrapper {
    flex-grow: 11
}

#button-wrapper {
    flex-grow: 1
}

#email-input { 
    width: 100%;
    height: 45px;
    border-radius: 100px;
    outline: none;
    border: none;
}

@media (min-width: 768px) and (max-width: 1024px) {
    .email {
        width: 100%;
    }

    .email-title {
        font-size: 20px !important;
    }

    .inputAndButton {
        flex-direction: column;
    }

    #input-wrapper {
        margin-bottom: 20px;
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .email {
        width: 100%;
    }

    .email-title {
        font-size: 20px !important;
    }

    .inputAndButton {
        flex-direction: column;
    }

    #input-wrapper {
        margin-bottom: 20px;
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .email {
        width: 100%;
    }

    .email-title {
        font-size: 20px !important;
    }

    .inputAndButton {
        flex-direction: column;
    }

    #input-wrapper {
        margin-bottom: 20px;
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .email {
        width: 100%;
    }

    .email-title {
        font-size: 20px !important;
    }

    .inputAndButton {
        flex-direction: column;
    }

    #input-wrapper {
        margin-bottom: 20px;
    }
}

</style>

