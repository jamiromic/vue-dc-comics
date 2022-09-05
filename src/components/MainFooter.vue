<template>
    <div>
        <div class="footer_top">
            <div class="services">
                <div class="service_item">
                    <img src="../assets/buy-comics-digital-comics.png" alt="Digital Comics App">
                    <a href="#">Digital Comics</a>
                </div>
                <div class="service_item">
                    <img src="../assets/buy-comics-merchandise.png" alt="Digital Comics Merchandise">
                    <a href="#">Dc Merchandise</a>
                </div>
                <div class="service_item">
                    <img src="../assets/buy-comics-subscriptions.png" alt="Digital Comics Subscriptions">
                    <a href="#">Subscription</a>
                </div>
                <div class="service_item">
                    <img src="../assets/buy-comics-shop-locator.png" alt="Digital Comics Shop Locator">
                    <a href="#">Comic Shop Locator</a>
                </div>
                <div class="service_item">
                    <img src="../assets/buy-dc-power-visa.svg" alt="Dc Power Visa">
                    <a href="#">Dc Power Visa</a>
                </div>
            </div>
        </div>
        <div class="footer_center">
            <div class="footer_lists">
                <div class="col">
                    <h4 class="title_list">DC COMICS</h4>
                        <ul class="singol_list">
                            <li>
                                <a href="#">Characters</a>
                            </li>
                            <li>
                                <a href="#">Comics</a>
                            </li>
                            <li>
                                <a href="#">Movies</a>
                            </li>
                            <li>
                                <a href="#">TV</a>
                            </li>
                            <li>
                                <a href="#">Games</a>
                            </li>
                            <li>
                                <a href="#">Videos</a>
                            </li>
                            <li>
                                <a href="#">News</a>
                            </li>                            
                        </ul>
                        <h4 class="title_list">SHOP</h4>
                        <ul class="singol_list">
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC Collectibles</a>
                            </li>                
                        </ul>
                </div>  
                <div class="col">
                    <h4 class="title_list">DC</h4>
                        <ul class="singol_list">
                            <li>
                                <a href="#">Terms Of Use</a>
                            </li>
                            <li>
                                <a href="#">Privacy Policy(New)</a>
                            </li>
                            <li>
                                <a href="#">AD Choices</a>
                            </li>
                            <li>
                                <a href="#">Advertising</a>
                            </li>
                            <li>
                                <a href="#">Subscriptions</a>
                            </li>
                            <li>
                                <a href="#">Talent Workshops</a>
                            </li>
                            <li>
                                <a href="#">CPSC Certificates</a>
                            </li>
                            <li>
                                <a href="#">Ratings</a>
                            </li>  
                            <li>
                                <a href="#">Shop Help</a>
                            </li>  
                            <li>
                                <a href="#">Contact Us</a>
                            </li>                              
                        </ul>
                </div>
                <div class="col">
                    <h4 class="title_list">SITES</h4>
                        <ul class="singol_list">
                            <li>
                                <a href="#">DC</a>
                            </li>
                            <li>
                                <a href="#">MAD Magazine</a>
                            </li>
                            <li>
                                <a href="#">Dc Kids</a>
                            </li>
                            <li>
                                <a href="#">DC Universe</a>
                            </li>
                            <li>
                                <a href="#">DC Power visa</a>
                            </li>                          
                        </ul>
                </div>
            </div>
            <div class="footer_picture_dc">
                <img src="../assets/dc-logo-bg.png" alt="Logo DC Bg">
            </div>

        </div>
        <div class="footer_bottom">

        </div>

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

    .footer_top {
        background-color: #0282F9;
        margin: 0 auto;
        padding: 3rem 14rem;
    }

    .services {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        gap: 2rem;

    }

    .service_item {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 60px;
        text-transform: uppercase;
        color: white;
        gap: 1rem;
    }


    img {
        height: 100%;
    }

    .footer_center {
        background-image: url(../assets/footer-bg.jpg);
        background-size: cover;
        display: flex;
        justify-content: space-around;
        padding: 0 15rem;
    }

    .footer_lists {
        display: flex;
        padding-top: 3rem;
    }

    .footer_picture_dc {
        margin-top: -50px;
    }

    .col {
        color: #959595;
        flex-grow: 1;
        flex-basis: 0;
        width: 170px;
        
        h4 {
            padding: 1rem 0;
            color: white;
            font-size: 1.25rem;
        }
    }

    li {
        padding-bottom: 5px;
    }

</style>