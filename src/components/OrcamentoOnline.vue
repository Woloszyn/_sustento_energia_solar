<template>
    <div id="orcamento_online">
        <div class="col-12">
            <div class="row titulo_orcamento">
                <div class="col-7">
                    <div class="module-tittle">QUERO GERAR MINHA ENERGIA</div>
                </div>
            </div>
            <div class="row orcamento">
                <div class="col-12">
                    <div class="col-7 module-text">
                        <div class="row">
                            <div class="col-12">
                                Contamos com uma equipe especializada para auxiliar você em todas as etapas
                                <br>
                                de seu projeto.
                                <b>Solicite um Orçamento!</b>
                            </div>
                        </div>
                        <form action="#">
                            <div class="row">
                                <div class="col-6">
                                    <input type="text" name="campo-1" class="form-control form-main-control--bd-color" placeholder="Nome">
                                    <input type="text" name="campo-2" class="form-control form-main-control--bd-color" placeholder="E-mail">
                                    <input type="text" name="campo-3" class="form-control form-main-control--bd-color" placeholder="Cidade">
                                    <input type="text" name="campo-4" class="form-control form-main-control--bd-color" placeholder="Telefone">
                                    <input type="text" name="campo-5" class="form-control form-main-control--bd-color" placeholder="Monofasico/ Bifasico/ Trifasico">
                                    <input type="text" name="campo-6" class="form-control form-main-control--bd-color" placeholder="Valor Médio da sua Conta de Energia">
                                    <button class="button_orcamento">SOLICITAR  ORÇAMENTO</button>
                                </div>
                                <div class="col-6">
                                    <textarea name="mensagem" id="mensagem" cols="30" rows="10" placeholder="Mensagem"></textarea>
                                </div>
                            </div>
                        </form>
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
        background-position-x: -50px;
        background-size: 120%;
        background-origin: border-box;
        min-height: 400px;
        background-repeat: no-repeat;
    }
    .titulo_orcamento {
        background-image: url('../assets/orcamento/title-orcamento-online.png');
        background-size: 100%;
        background-repeat: no-repeat;
    }
    .module-tittle {
        font-size: 26px;
        font-weight: 700;
        font-style: italic;
    }
    .module-text {
        font-size: 16px;
        font-style: italic;
    }
    .form-control {
        font-size: 15px;
        line-height: 16px;
        height: 42px;
        padding: 15px 20px;
        border: 1px solid transparent;
        border-radius: 50px;
        box-shadow: 0 3px 6px rgb(0 0 0 / 15%);
        margin-top: 15px;
    }
    .button_orcamento {
        background-color: #3baa34;
        border-radius: 50px;
        border: 1px solid transparent;
        box-shadow: 0 3px 6px rgb(0 0 0 / 15%);
        padding: 10px 20px;
        font-size: 15px;
        line-height: 16px;
        height: 42px;
        color: #fff;
        text-transform: uppercase;
        font-weight: bold;
        margin-top: 15px;
    }
    #mensagem {
        height: 332px;
        font-size: 15px;
        line-height: 16px;
        padding: 15px 20px;
        border: 1px solid transparent;
        box-shadow: 0 3px 6px rgb(0 0 0 / 15%);
        border-radius: 30px;
    }

</style>