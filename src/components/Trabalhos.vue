<template>
    <div id="trabalhos">
        <div class="row">
            <div class="col-4 titulo">
                <h1 class="trabalhos_titulo">
                    Trabalhos
                </h1>
                <div class="row">
                    <div class="col-6">
                        <img src="../assets/trabalhos/clique.png" alt="" srcset="">
                    </div>
                </div>
            </div>
            <div class="col-6 imagens">
                <div class="images" v-viewer>
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho1.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho2.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho3.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho4.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho5.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho6.jpg">
                </div>
                <viewer :images="images">
                </viewer>
            </div>
            <div class="col-2"></div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            images: ['../assets/parceiros/apsistems.jpeg', '../assets/parceiros/byd.jpeg']   
        }
    },
}
</script>

<style>
    #trabalhos {
        background-image: url('../assets/trabalhos/background-trabalhos.jpeg');
        min-height: 80vh;
        padding-top: 50px;
    }
    .trabalhos_titulo {
        color: white;
    }
    .titulo {
        background-image: url('../assets/orcamento/title-orcamento-online.png');
        min-height: 450px;
        background-size: 300%;
        background-position-y: ß250px;
        background-position-x: -325px;
        background-repeat: no-repeat;
        background-position-y: top;
    }
    .imagem_grid {
        width: 250px;
    }
</style>