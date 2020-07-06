<template>
    <div class="services">
        <div class="services-group">
            <div data-aos="fade" class="services-group-item ">
                <div><img height="200" width="250" src="../assets/images/responsive.png" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Aplicaciones responsive</span>
                    <br/>
                    <span class="size-15">Mira tus sitios o web apps desde cualquier dispositivo. Utilizamos frameworks de última generación para lograr apps flexibles a los cambios.</span>
                </div>
            </div>
            <div data-aos="fade" class="services-group-item ">
                <div><img height="200" width="200" src="../assets/images/ssl.png" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Seguridad SSL</span>
                    <br/>
                    <span class="size-15">Todas nuestras tiendas poseen certificado SSL para garantizar la mejor seguridad en las transacciones.</span>
                </div>
            </div>            
        </div>
        <div class="services-group">
            <div data-aos="fade" class="services-group-item ">
                <div><img height="200" width="200" src="../assets/images/capacitacion.png" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Capacitación online</span>
                    <br/>
                    <span class="size-15">Nunca entregaremos un desarrollo sin antes haberte brindado una capacitación online para comentarte el uso de cada app y sacarte todas las dudas.</span>
                </div>
            </div>
            <div data-aos="fade" class="services-group-item ">
                <div><img height="200" width="200" src="../assets/images/online-store.png" alt=""></div>
                <div class="y-20 item-description">
                    <span class="bold">Tener una tienda online nunca fue tan facil!</span>
                    <br/>
                    <span class="size-15">Creamos tu tienda online, linkeamos mercadopago para recibir pagos y capacitamos a nuestros clientes para el uso de la misma.</span>
                </div>
            </div>   
        </div>
    </div>
</template>

<style scoped>
* { color: white; text-align: center }

.services {   
    display: flex;
    flex-direction: column;    
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

