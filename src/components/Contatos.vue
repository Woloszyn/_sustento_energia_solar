<template>
    <div id="contatos">
        <div class="col-12"> 
            <div class="row contato_bg">
                <div class="col-12">
                    <div class="tituloContato">Contato</div>
                </div>
                <div class="col-12">
                    <div class="row">
                        <div class="col-4 sustentaSaoCarlos">Sustento Energia - São Carlos Rua Aquidaban, 1 Centro, São Carlos/SP - CEP 13.560-120</div>
                        <div class="col-4 whatsApp">
                            <i class="fab fa-whatsapp-square"></i>
                            <a href="https://web.whatsapp.com/send?phone=5517981907484&amp;text=Olá!" target="_blank" class="whatsApp"><i class="fab fa-whatsapp"></i> (17) 98190-7484</a>
                        </div>
                        <div class="col-4 email">contato@sustentoenergiasolar.com.br</div>
                    </div>
                    <div class="row">
                        <div class="col-4 sustentaCatanduva">Sustento Energia - Catanduva
                            Rua Ribeirão Preto, 411 Vila Rodrigues, Catanduva/SP - CEP 15.801-340
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col-12">
            <div class="row">
                <div class="col-6">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d59178.62969681153!2d-47.894441!3d-22.024168!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x837f2e453345767f!2sSustento%20Energia%20Solar%C2%AE!5e0!3m2!1spt-BR!2sbr!4v1641667887866!5m2!1spt-BR!2sbr" width="100%" allowfullscreen="" loading="lazy" class="mapa"></iframe>
                </div>
                <div class="col-6">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d14885.893770303397!2d-48.980548!3d-21.133549!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94bc1e60064f80a5%3A0xe3c22b22b6a45c20!2sR.%20Ribeir%C3%A3o%20Preto%2C%20411%20-%20Vila%20Rodrigues%2C%20Catanduva%20-%20SP%2C%2015801-340!5e0!3m2!1spt-BR!2sbr!4v1641667795697!5m2!1spt-BR!2sbr" width="100%" allowfullscreen="" loading="lazy" class="mapa"></iframe>
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
    .contato_bg {
        background-image: url('../assets/contatos/bg-contatos.jpg') ;
        background-position-x: -250px;
        background-size: 150%;
        background-origin: border-box;
        margin-top: 10px;
        min-height: 700px;
        background-repeat: no-repeat;
    }
    .mapa {
        height: 200px;
        border: #4ea103 2px solid;
        border-radius: 0px;
        margin-bottom: 45px;
    }
    .tituloContato {
        display: inline-block;
        color: #fff;
        padding: 12px 38px 7px;
        border: #4ea103 3px solid;
        border-radius: 30px;
        margin-bottom: 45px;
        font-size: 26px;
        font-weight: 700;
        font-style: italic;
        text-transform: uppercase;
    }
    .sustentaSaoCarlos {
        background-position: left 10px;
        padding-left: 50px;
        min-height: 48px;
        padding-top: 12px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
    }
    .whatsApp:hover {
        color: #fff;
    }
    .whatsApp {
        color: #fff;
        text-decoration: none;
        font-style: italic;
        font-weight: lighter;
    }
    .email {
        color: #fff;
        font-style: italic;
        font-weight: lighter;
    }
    .sustentaCatanduva {
        background-position: left 10px;
        padding-left: 50px;
        min-height: 48px;
        padding-top: 12px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
    }
</style>