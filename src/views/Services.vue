<template>
    <div class="services">
        <div class="services-group">
            <div data-aos="fade" class="services-group-item ">
                <div><img src="../assets/images/icon-access-anywhere.svg" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Access your files, anywere</span>
                    <br/>
                    <span class="size-15">The ability to use a smartphone, tablet, or computer to access your account emans your files follow you everywhere.</span>
                </div>
            </div>
            <div data-aos="fade" class="services-group-item ">
                <div><img src="../assets/images/icon-security.svg" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Security you can trust</span>
                    <br/>
                    <span class="size-15">2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.</span>
                </div>
            </div>            
        </div>
        <div class="services-group">
            <div data-aos="fade" class="services-group-item ">
                <div><img src="../assets/images/icon-collaboration.svg" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Real-time collaboration</span>
                    <br/>
                    <span class="size-15">Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required</span>
                </div>
            </div>
            <div data-aos="fade" class="services-group-item ">
                <div><img src="../assets/images/icon-any-file.svg" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Store any type of file</span>
                    <br/>
                    <span class="size-15">Whether you're sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.</span>
                </div>
            </div>   
        </div>
    </div>
</template>

<style scoped>
* { color: white; text-align: center }

.services {
    /* background: #e1efbb url('../assets/images/bg-curvy-desktop.svg'); */
    display: flex;
    flex-direction: column;
    padding: 50px 200px 50px 200px;
}

.services-group {
    display: flex;
    flex-direction: row
}

.services-group-item {
    display: flex;
    flex-direction: column;
    padding: 30px;
}

@media (min-width: 768px) and (max-width: 1024px) {
    .services {
        padding: 0
    }

    .services-group {
        flex-direction: column;
        padding-top: 40px;
    }

    .services-group-item {
        padding: 20px;
    }

    .item-description span:first-of-type {
        font-size: 20px;
    }


}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .services {
        padding: 0
    }

    .services-group {
        flex-direction: column;
        padding-top: 40px;
    }

    .services-group-item {
        padding: 20px;
    }

    .item-description span:first-of-type {
        font-size: 20px;
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .services {
        padding: 0
    }

    .services-group {
        flex-direction: column;
        padding-top: 40px;
    }

    .item-description span:first-of-type {
        font-size: 20px;
    }

    .services-group-item {
        padding: 20px;
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .services {
        padding: 0
    }

    .services-group {
        flex-direction: column;
        padding-top: 40px;
    }

    .item-description span:first-of-type {
        font-size: 20px;
    }

    .services-group-item {
        padding: 20px;
    }
}

</style>

