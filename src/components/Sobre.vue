<template>
    <div id="sobre">
        <div class="col-12">
            <div class="row bg-sobre">
                <div class="row bg_titulo">
                    <div class="col-lg-7 col-md-12 col-12">
                        <div class="module-tittle">QUEM SOMOS E O QUE FAZEMOS</div>
                    </div>
                </div>
                    <div class="col-2"></div>
                    <div class="col-md-10 col-lg-4 col-10 texto">
                        <p>Somos uma empresa focada em sustentabilidade <br> 
                            energética. Nosso diferencial é uma forte base técnica em <br> 
                            elaboração e viabilidade de projetos. Trabalhamos com <br> 
                            microgeração de energia e desenvolvemos softwares para <br>
                            o mercado de energia solar.
                        </p>
                        <p>
                            Nossa equipe de TI é direcionada a otimizar todos os <br>
                            processos internos e construir uma base tecnológica <br>
                            completa para todo setor energético. Além disso, <br>
                            desenvolvemos softwares para qualquer empresa do setor <br>
                            que esteja interessada em nossos serviços.
                        </p>
                        <p>
                            O objetivo é melhorar ao máximo o consumo de energia, <br>
                            criar fontes limpas por meio de microgeração/minigeração <br>
                            e aproximar as geradoras dos consumidores para evitar <br>
                            grandes perdas no transporte energético.
                        </p>
                    </div>
                    <div class="col-lg-4 col-12">
                        <div class="row">
                            <div class="row">
                                <div class="col-lg-6 col-md-6 col-12">
                                    <img src="../assets/sobre/balao1.png">
                                </div>
                                <div class="col-lg-6 col-md-6 col-12">
                                    <img src="../assets/sobre/balao2.png">
                                </div>
                            </div>
                            <div class="row">
                                <div class="col-lg-6 col-md-6 col-12">
                                    <img src="../assets/sobre/balao3.png">
                                </div>
                                <div class="col-lg-6 col-md-6 col-12">
                                    <img src="../assets/sobre/balao4.png">
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-2"></div>
                    <div class="row">
                        <div class="col-12">
                            <span class=" col-12 col-md-6 float-right">
                                <center><img src="../assets/sobre/balao5.png" alt="" srcset=""></center>
                            </span>
                            <img src="../assets/sobre/sobre-text.png" class="tamanhoImagem">
                        </div>
                    </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.bg-sobre {
    background-image: url('../assets/sobre/bg-sobre.jpg') ;
    background-position: center center;
    background-size: cover;
    background-origin: border-box;
    min-height: 550px;
    background-repeat: no-repeat;
}

.module-tittle {
    font-weight: 700;
    font-style: italic;
}

@media(max-width: 820px) {
    .float-right{
        float: none;
    }
}

.float-right {
    float: right;
}
.texto {
    color: #000;
    font-style: italic;
    font-weight: 500;
    font-size: 15px;
    text-align: left;
}
.tamanhoImagem {
    padding: 30px;
}
</style>