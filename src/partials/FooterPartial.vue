<template>
    <div class="footer">
        <div id="footer-about">
            <div id="logo">
                <img src="../assets/images/logo.svg" alt="">
            </div>
            <div id="footer-text">
                <p>
                    Lorem ipsum dolor sit amet consectetur, <br> adipisicing elit. Optio non dolor possimus, hic <br>
                    Lorem ipsum dolor sit amet consectetur
                </p>
            </div>
        </div>
        <div id="footer-contact">
            <div><span>+1-543-123-4567</span></div>
            <div><span>example@fylo.com</span></div>
        </div>
        <div class="links-list">
            <ul>
                <li>About Us</li>
                <li>Jobs</li>
                <li>Press</li>
                <li>Blog</li>
            </ul>
        </div>
        <div class="links-list">
            <ul>
                <li>Contact Us</li>
                <li>Terms</li>
                <li>Privacy</li>
                <li>Feedback</li>
            </ul>
        </div>            
        <div id="footer-social-networks"></div>
    </div>
</template>

<style scoped>
* {
    color: white
}
.footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 100px 50px 100px 50px;
    flex-grow: 1;
    background: hsl(216, 53%, 9%);
}

.footer-about {
    display: flex;
    flex-direction: column;
    flex-grow: 2;
}

ul {
    list-style: none;
}

ul > li {
    padding-top: 20px;
    cursor: pointer;
}

@media (min-width: 768px) and (max-width: 1024px) {
    .footer {
        flex-direction: column;
        padding: 200px 50px 100px 50px;
        align-items: flex-start
    }

    ul {
        padding: 0
    }
}

@media (min-width: 768px) and (max-width: 1024px) and (orientation: landscape) {
    .footer {
        flex-direction: column;
        padding: 200px 50px 100px 50px;
        align-items: flex-start
    }

    ul {
        padding: 0
    }
}

@media (min-width: 481px) and (max-width: 767px) {
    .footer {
        flex-direction: column;
        padding: 200px 50px 100px 50px;
        align-items: flex-start
    }

    ul {
        padding: 0
    }
}

@media (min-width: 320px) and (max-width: 480px) {
    .footer {
        flex-direction: column;
        padding: 200px 50px 100px 50px;
        align-items: flex-start
    }

    ul {
        padding: 0
    }
}

</style>

