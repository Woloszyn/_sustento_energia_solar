<template>
    <div id="como_funciona">
        <div class="col-12 main_container">
            <div class="row bg_titulo">
                <div class="col-lg-7 col-md-12 col-12">
                    <div class="module-tittle">O SISTEMA FUNCIONA ASSIM</div>
                </div>
            </div>
        </div>
        <div class="col-11">
            <div class="row">
                <div class="col-2"></div>
                <div class="col-lg-4 col-md-10 col-10 ">
                    <img class="funcionamento_imagem" src="../assets/orcamento/funcionamento-min.jpg" alt="">
                </div>
                <div class="col-2">
                </div>
                <div class="col-md-8 col-lg-4 col-8">
                    <center>
                        <div class="paragrafos">
                            <p>A energia solar funciona por meio da irradiação solar, ou seja, pela luminosidade solar e não por meio do seu calor. 
                                Basicamente, quanto mais ensolarado e claro o dia, mais energia é gerada.
                            </p>
                            <p>
                                Os módulos fotovoltaicos, popularmente chamados de painéis,
                                recebem a irradiação solar e transformam a luz do sol em energia elétrica.
                            </p>
                            <p>
                                A energia gerada passa por um inversor, ou microinversor, que a iguala ao tipo de corrente que recebemos da rede pública. Deste modo, nos beneficiamos da energia solar e compensamos da conta de energia a quantidade produzida pelos módulos. 
                                Assim, é possível até compartilhá-la entre contas de energias cadastradas no mesmo CPF ou CNPJ.
                            </p>
                        </div>
                    </center>
                </div>
                <div class="col-2"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
    .tituloComoFunciona {
        background-image: url('../assets/orcamento/title-orcamento-online.png');
        background-size: 100%;
        background-repeat: no-repeat;
        height: 90px;
    }
    .funcionamento_imagem {
        max-width: 100%;
    }
    .paragrafos {
        color: #000;
        font-style: italic;
        font-weight: 500;
        font-size: 16px;
        text-align: left;
    }
    .main_container {
        padding-top: 40px;
    }
</style>