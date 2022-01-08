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
                <VueSlickCarousel :autoplay='true' :slidesToShow='6' :arrows="true" :dots="true">
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
    .parceiros {
        background-color: white;
        border: 1px solid transparent;
        border-radius: 10px;
        border-top: 1px solid rgba(0, 0, 0, 0.199);
        width: 180px !important;
        box-shadow: 1px 1px 1px 1px rgba(0,0,0,0.5); 
        justify-content: center;
    }
    .textoProdutosParceiros {
        font-style: italic;
        color: #212529;
        font-size: 18px;
    }
</style>