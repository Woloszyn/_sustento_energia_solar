<template>
    <div id="orcamento_online">
        <div class="col-12 main_container">
            <div class="row bg_titulo">
                <div class="col-lg-7 col-md-12 col-12">
                    <div class="module-tittle">QUERO GERAR MINHA ENERGIA</div>
                </div>
            </div>
            <div class="row orcamento">
                <div class="col-12">
                    <div class="col-lg-7 col-md-12 col-12 module-text">
                        <div class="row">
                            <div class="col-lg-2 col-1"></div>
                            <div class="col-lg-8 col-10">
                                <span class="subtitulo">
                                    Contamos com uma equipe especializada para auxiliar você em todas as etapas 
                                    de seu projeto.
                                    <b>Solicite um Orçamento!</b>
                                </span>
                            </div>
                            <div class="col-lg-2 col-1"></div>
                        </div>
                        <div class="row">
                            <div class="col-lg-2 col-1"></div>
                            <div class="col-lg-4 col-md-12 col-12">
                                <input type="text" name="campo-1" class="form-control2" placeholder="Nome">
                                <input type="text" name="campo-2" class="form-control2" placeholder="E-mail">
                                <input type="text" name="campo-3" class="form-control2" placeholder="Cidade">
                                <input type="text" name="campo-4" class="form-control2" placeholder="Telefone">
                                <input type="text" name="campo-5" class="form-control2" placeholder="Monofasico/ Bifasico/ Trifasico">
                                <input type="text" name="campo-6" class="form-control2" placeholder="Valor Médio da sua Conta de Energia">
                            </div>
                            <div class="col-lg-6 col-md-12 col-12">
                                <textarea name="mensagem" id="mensagem" cols="30" rows="10" placeholder="Mensagem"></textarea>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col-lg-2 col-1"></div>
                            <div class="col-lg-4 col-md-12 col-12">
                                <button class="button_orcamento">SOLICITAR  ORÇAMENTO</button>
                            </div>
                        </div>
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

    .orcamento{
        background-image: url('../assets/orcamento/bg-orcamento.jpg') ;
        background-size: cover;
        background-position: center center;
        min-height: 550px;
        padding-bottom: 50px;
        background-repeat: no-repeat;
    }
    @media(max-width: 986px) {
        .bg_titulo {
            background: none !important;
        }
        .module-tittle {
            border: 3px solid green;
            border-radius: 30px;
            max-width: 90% !important;
            margin: 20px;
            font-weight: 700;
            padding: 15px;
        }
        .clique_aqui {
            display: none !important;
        }
        .module-text {
            margin: 15px;
        }
    }

    .bg_titulo {
        background-image: url('../assets/orcamento/title-orcamento-online.png');
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center left;
        min-height: 50px;
    }
    .module-tittle {
        font-size: 30px !important;
        font-style: italic;
    }
    .module-text {
        font-size: 16px;
        font-style: italic;
        text-align: left;
    }
    .form-control2 {
        font-size: 15px;
        line-height: 16px;
        height: 42px;
        padding: 15px 20px;
        border: 1px solid transparent;
        border-radius: 50px;
        box-shadow: 0 3px 6px rgb(0 0 0 / 15%);
        margin-top: 15px;
        width: calc(100% - 30px);
        color: #495057;
        background-color: #fff;
        background-clip: padding-box;
    }
    .button_orcamento {
        background-color: #3baa34;
        border-radius: 50px;
        border: 1px solid transparent;
        box-shadow: 0 3px 6px rgb(0 0 0 / 15%);
        padding: 10px 20px;
        font-size: 15px;
        width: calc(100% - 30px);
        line-height: 16px;
        height: 42px;
        color: #fff;
        text-transform: uppercase;
        font-weight: bold;
        margin-top: 15px;
    }
    #mensagem {
        min-height: 23vw;
        font-size: 15px;
        line-height: 16px;
        padding: 15px 20px;
        border: 1px solid transparent;
        box-shadow: 0 3px 6px rgb(0 0 0 / 15%);
        resize: none;
        margin-top: 15px;
        border-radius: 30px;
        width: calc(100% - 30px);
    }
    .main_container {
        padding-top: 60px;
    }
    .subtitulo {
        margin-bottom: 30px;
        font-size: 16px;
        font-style: italic;
        text-align: left;
        font-weight: 500;
        padding-bottom: 30px;
    }
</style>