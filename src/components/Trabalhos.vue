<template>
    <div id="trabalhos">
        <div class="row">
            <div class="col-lg-4 col-md-12 col-12">
                <div class="row bg_titulo bg_titulo_trabalho cor_branca">
                    <div class="module-tittle">Trabalhos</div>
                </div>
                <div class="row clique_aqui">
                    <div class="col-12">
                        <center><img src="../assets/trabalhos/clique.png" alt="" srcset=""></center>
                    </div>
                </div>
            </div>
            <div class="col-md-12 col-lg-6 col-12 imagens">
                <div class="images" v-viewer>
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho1.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho2.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho3.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho4.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho6.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho7.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho8.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho9.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho10.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho11.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho12.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho13.jpg">
                    <img class="imagem_grid" src="../assets/trabalhos/trabalho14.jpg">
                </div>
            </div>
            <div class="col-2"></div>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style>
    #trabalhos {
        background-image: url('../assets/trabalhos/background-trabalhos.jpeg');
        min-height: 80vh;
        width: 100% !important;
        background-repeat: no-repeat;
        background-position: center center;
        padding-top: 50px;
        padding-bottom: 50px;
        -webkit-background-size: cover;
        -moz-background-size: cover;
        -o-background-size: cover;
        background-size: cover;
    }
    .bg_titulo_trabalho {
        background-position-x: 35% !important;
    }
    .cor_branca {
        color: white;
    }
    .imagem_grid {
        width: 30%;
    }
</style>