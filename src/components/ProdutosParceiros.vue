<template>
    <div id="produtos_e_parceiros">
        <div class="col-12">
            <div class="row produtos_parceiros">
                <div class="col-6">
                    <div class="module-tittle"><b>PRODUTOS E PARCEIROS</b></div>
                </div>
                <div class="col-6">
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
                <VueSlickCarousel :autoplay='true' :slidesToShow='6' dotsClass='pontosCarousel' :arrows="true" :dots="true">
                    <div class="parceiros shine-me">
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
    .produtos_parceiros{
        background-image: url('../assets/orcamento/title-orcamento-online.png');
        background-size: 110%;
        min-height: 60px;
        max-width: 70%;
        background-repeat: no-repeat;
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
        width: 180px !important;
        box-shadow: 1px 2px 4px rgba(0,0,0,0.5); 
        justify-content: center;
    }

    .textoProdutosParceiros {
        font-style: italic;
        color: #212529;
        font-size: 18px;
    }
</style>