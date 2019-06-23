<template>
    <div class="offer">
        <div data-aos="fade-right">
            <img class="responsive-img" src="../assets/images/illustration-stay-productive.png" alt="stay productive with fylo">
        </div>
        <div data-aos="fade-left" id="offer-info">
            <div><span class="bold white size-35">Stay productive, <br/> wherever you are</span></div>
            <br />
            <div>
                <span class="white">Never let location be an issue when accessing your files. Fylo has you covered for all of your file storage needs.</span>
                <br /><br />
                <span class="white">Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.</span>
                <br /><br />
                <a href="/" id="link-fylo-work">See how Fylo works</a>
            </div>
        </div>
    </div>    
</template>

<style>
.offer {
    display: flex;
    text-align: left;
    justify-content: center;
    align-items: center;
    padding: 50px 100px 50px 100px;
}

.offer-info {
    display: flex;
}

#link-fylo-work {
    color: hsl(176, 68%, 64%);
}

@media (min-width: 768px) and (max-width: 1024px) {
    .offer {
        flex-direction: column;
        padding: 60px 40px 60px 40px;
    }

    #offer-info {
        padding-top: 40px;
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .offer {
        flex-direction: column;
        padding: 80px 30px 80px 30px;
    }

    #offer-info {
        padding-top: 40px;
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .offer {
        flex-direction: column;
        padding: 80px 30px 80px 30px;
    }

    #offer-info {
        padding-top: 40px;
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .offer {
        flex-direction: column;
        padding: 80px 30px 80px 30px;
    }

    #offer-info {
        padding-top: 40px;
    }
}

</style>

