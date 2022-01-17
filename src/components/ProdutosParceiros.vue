<template>
    <div id="produtos_e_parceiros">
        <div class="col-12">
            <div class="row produtos_parceiros">
                <div class="col-lg-7 col-md-12 col-12 bg_titulo">
                    <div class="module-tittle">Produtos Parceiros</div>
                </div>
                <div class="col-lg-5 col-md-12 col-12">
                    <div class="textoProdutosParceiros">
                        Conheça nossos parceiros e produtos que trabalhamos.
                    </div>
                </div>
            </div>
        </div>
        <hr class="sem_background">
        <div class="row">
            <div class="col-1"></div>
            <div class="col-10">
                <VueSlickCarousel v-bind="settings">
                    <div class="parceiros">
                        <center>
                            <img src="../assets/parceiros/ecori.jpeg" title="Ecori">
                        </center>
                    </div>
                    <div class="parceiros">
                        <center>
                            <img src="../assets/parceiros/solar-edge.jpeg" title="Solar Edge">
                        </center>
                    </div>
                    <div class="parceiros">
                        <center>
                            <img src="../assets/parceiros/canadian-solar.jpeg" title="Canadian Solar">
                        </center>
                    </div>
                    <div class="parceiros">
                        <center>
                            <img src="../assets/parceiros/talesun.jpeg" title="Talesun">
                        </center>
                    </div>
                    <div class="parceiros">
                        <center>
                            <img src="../assets/parceiros/apsistems.jpeg" title="APSystems">
                        </center>
                    </div>
                    <div class="parceiros">
                        <center>
                            <img src="../assets/parceiros/byd.jpeg" title="BYD">
                        </center>
                    </div>
                    <div class="parceiros">
                        <center>
                            <img src="../assets/parceiros/dahsolar.jpeg" title="DAH solar">
                        </center>
                    </div>
                </VueSlickCarousel>
            </div>
            <div class="col-1">
            </div>
        </div>
    </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
    data: ()  => {
        return {
            settings: {
                "dots": true,
                "autoPlay": true,
                "infinite": true,
                "speed": 500,
                "dotsClass": "pontosCarousel",
                "slidesToShow": 6,
                "slidesToScroll": 6,
                "initialSlide": 0,
                "responsive": [
                    {
                    "breakpoint": 1024,
                    "settings": {
                        "slidesToShow": 3,
                        "slidesToScroll": 3,
                        "infinite": true,
                        "dots": true
                    }
                    },
                    {
                    "breakpoint": 600,
                    "settings": {
                        "slidesToShow": 2,
                        "slidesToScroll": 2,
                        "initialSlide": 2
                    }
                    },
                    {
                    "breakpoint": 480,
                    "settings": {
                        "slidesToShow": 1,
                        "slidesToScroll": 1
                    }
                    }
                ]
            }
        }
    },
    components: { VueSlickCarousel },
}
</script>

<style>
    #produtos_e_parceiros {
        background-color: rgba(128, 128, 128, 0.192);
        padding-top: 40px;
        min-height: 300px;
    }
    .pontosCarousel {
        padding-top: 20px;
        list-style: circle;
        display: flex !important;
        justify-content: center;
        flex-direction: row;
    }
    .pontosCarousel > .slick-active {
        list-style: disc;
        color: green;
    }
    .pontosCarousel > li {
        font-size: 45px;
        color: rgb(179, 178, 178);
        padding-right: 14px;
        cursor: pointer;
    }
    button.slick-next:before {
        color: green;
        font-family: "Font Awesome 5 Free";
        font-weight: 900;
        font-size: 30px;
        content: "\f054";
    }
    @media(max-width:800px) {
        button.slick-prev:before{
            display: none !important;
        }
        button.slick-next:before{
            display: none !important;
        }
    }
    .slick-prev {
        top: 60px;
        left: -35px;
    }
    .slick-next {
        top: 60px;
        right: -35px;
    }
    button.slick-prev:before{
        color: green;
        font-size: 30px;
        font-family: "Font Awesome 5 Free";
        font-weight: 900;
        content: "\f053";
    }
    .pontosCarousel > li > button {
        background-color: transparent;
        color: transparent;
        width: 15px;
        border: none;
    }
    .parceiros {
        background-color: white;
        border: 1px solid transparent;
        border-radius: 10px;
        border-top: 1px solid rgba(0, 0, 0, 0.199);
        min-width: 15% !important;
        box-shadow: 1px 2px 4px rgba(0,0,0,0.5); 
        justify-content: center;
    }

    .textoProdutosParceiros {
        font-style: italic;
        color: #212529;
        font-size: 18px;
    }
</style>