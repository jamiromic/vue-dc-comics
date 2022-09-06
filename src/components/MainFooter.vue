<template>
    <div>
        <div class="footer_top">
            <div class="services">
                <div v-for="(item,i) in dataOptions" :key="i" class="service_item">
                    <img :src="item.img" :alt="item.name">
                    <a href="#">{{ item.name }}</a>
                </div>
            </div>
        </div>
        <div class="footer_center">
            <div class="footer_lists">
                <div class="col">
                    <h4 class="title_list">DC COMICS</h4>
                        <ul class="singol_list">
                            <li v-for="(item,i) in dataLink" :key="i">
                                <a href="#">{{ item }}</a>
                            </li>       
                        </ul>
                        <h4 class="title_list">SHOP</h4>
                        <ul class="singol_list">
                            <li v-for="(item,i) in dataLink2" :key="i">
                                <a href="#">{{ item }}</a>
                            </li>               
                        </ul>
                </div>  
                <div class="col">
                    <h4 class="title_list">DC</h4>
                        <ul class="singol_list">
                            <li v-for="(item,i) in dataLink3" :key="i">
                                <a href="#">{{ item }}</a>
                            </li>                     
                        </ul>
                </div>
                <div class="col">
                    <h4 class="title_list">SITES</h4>
                        <ul class="singol_list">
                            <li v-for="(item,i) in dataLink4" :key="i">
                                <a href="#">{{ item }}</a>
                            </li>                  
                        </ul>
                </div>
            </div>
            <div class="footer_picture_dc">
                <img src="../assets/dc-logo-bg.png" alt="Logo DC Bg">
            </div>

        </div>
        <div class="footer_bottom">
            <button type="submit">SIGN-UP NOW!</button>
            <ul class="list_icons">
                <h4>FOLLOW US</h4>
                <li v-for="(item,i) in dataSocial" :key="i">
                    <img :src="item.img" :alt="item.name">
                </li>
            </ul>

        </div>

    </div>
</template>

<script>
    import dataOptions from '../dataOptions';
    import dataLink from '../dataLink'; 
    import dataLink2 from '../dataLink2';
    import dataLink3 from '../dataLink3';
    import dataLink4 from '../dataLink4';
    import dataSocial from '../dataSocial';

    export default {
        components: {  
    },
    data() {
        return {
            dataOptions: dataOptions,
            dataLink: dataLink,
            dataLink2: dataLink2,
            dataLink3: dataLink3,
            dataLink4: dataLink4,
            dataSocial: dataSocial
            
        }
    }
        
    }
</script>

<style lang="scss" scoped>

    .footer_top {
        background-color: #0282F9;
        margin: 0 auto;
        padding: 3rem 17rem;
        position: relative;
    }

    .services {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        gap: 4rem;

    }

    .service_item {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 50px;
        text-transform: uppercase;
        color: white;
        gap: 1rem;
        font-size: 0.75rem;
    }


    img {
        height: 100%;
    }

    .footer_center {
        background-image: url(../assets/footer-bg.jpg);
        background-size: cover;
        display: flex;
        justify-content: space-around;
        padding: 0 12rem;
        height: 360px;
    }

    .footer_lists {
        display: flex;
        padding-top: 1.5rem;
    }

    .footer_picture_dc {
        margin-top: -100px;
        margin-bottom: -100px;
    }

    .col {
        color: #959595;
        flex-grow: 1;
        flex-basis: 0;
        width: 130px;
        font-size: 0.75rem;
        
        h4 {
            padding: 1rem 0;
            color: white;
            font-size: 1rem;
        }
    }

    li {
        padding-bottom: 5px;
    }

    .footer_bottom {
        display: flex;
        justify-content: space-between;
        padding: 2rem 18rem;
        background-color: #303030;
        flex-wrap: wrap;
        position: relative;

        button {
            height: 45px;
            align-self: center;
            border: 2px solid #0282F9;
            background-color: #303030;
            color: white;
            padding: 0 0.75rem;
        }

        .list_icons{
            display: flex;
            align-items: center;
            flex-wrap: wrap;
            gap: 1rem;

            h4 {
                padding-right: 0.75rem;
                color: #0282F9;
                
            }

            li {
                width: 2.5rem;
                height: 2.5rem;
            }

        
        }
    }

</style>