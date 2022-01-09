<template>
    <div id="contatos">
        <div class="col-12"> 
            <div class="row contato_bg">
                <div class="col-12">
                    <div class="tituloContato">Contato</div>
                </div>
                <div class="col-12">
                    <div class="row">
                        <div class="col-4">
                            <div class="sustentaSaoCarlos">
                                <i class="fas fa-map-marker-alt iconeLocalizacao"></i> Sustento Energia - São Carlos
                            </div>
                            <div class="estiloRuaAquidaban">
                                Rua Aquidaban, 1 Centro, São Carlos/SP
                            </div>
                            <div class="estiloRuaCep">- CEP 13.560-120</div>
                        </div>
                        <div class="col-4 whatsApp">
                            <a href="https://web.whatsapp.com/send?phone=5517981907484&amp;text=Olá!" target="_blank" class="whatsApp"><i class="fab fa-whatsapp"></i> (17) 98190-7484</a>
                        </div>
                        <div class="col-4 email"><i class="fas fa-envelope"></i> contato@sustentoenergiasolar.com.br</div>
                    </div>
                    <div class="row">
                        <div class="col-5">
                            <div class="sustentaCatanduva">
                                <i class="fas fa-map-marker-alt iconeLocalizacao"></i> Sustento Energia - Catanduva
                            </div>
                            <div class="estiloRuaCep">
                                Rua Ribeirão Preto, 411 Vila Rodrigues, Catanduva/SP
                            </div>
                            <div class="estiloRuaCep">
                                - CEP 15.801-340
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="col-12">
            <div class="row">
                <div class="col-6 paddingZero">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d59178.62969681153!2d-47.894441!3d-22.024168!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x837f2e453345767f!2sSustento%20Energia%20Solar%C2%AE!5e0!3m2!1spt-BR!2sbr!4v1641667887866!5m2!1spt-BR!2sbr" width="100%" allowfullscreen="" loading="lazy" class="mapa"></iframe>
                </div>
                <div class="col-6 paddingZero">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d14885.893770303397!2d-48.980548!3d-21.133549!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94bc1e60064f80a5%3A0xe3c22b22b6a45c20!2sR.%20Ribeir%C3%A3o%20Preto%2C%20411%20-%20Vila%20Rodrigues%2C%20Catanduva%20-%20SP%2C%2015801-340!5e0!3m2!1spt-BR!2sbr!4v1641667795697!5m2!1spt-BR!2sbr" width="100%" allowfullscreen="" loading="lazy" class="mapa"></iframe>
                </div>
            </div>
        </div>
        <div class="col-12">
            <div class="row redeSociais_bg">
                <div class="row">
                    <div class="col-4">
                        <img src="../assets/contatos/logo-sustento.png" alt="">
                    </div>
                    <div class="col-4">
                        <div class="sustentaSaoCarlosFinal">
                            Sustento Energia - São Carlos
                        </div>
                        <div class="estiloRuaAquidaban">
                            Rua Aquidaban, 1 Centro - São Carlos/SP 
                        </div>
                        <div class="sustentaSaoCarlosFinal">
                            Sustento Energia - Catanduva
                        </div>
                        <div class="estiloRuaRibeirao">
                            Rua Ribeirão Preto, 411 Vila Rodrigues - Catanduva/SP 
                        </div>
                        <div class="whatsApp">
                            <a href="https://web.whatsapp.com/send?phone=5517981907484&amp;text=Olá!" target="_blank" class="whatsApp">
                                Whatsapp: (17) 98190-7484
                            </a>
                        </div>
                        <div class="estiloEmail">
                            E-mail: contato@sustentoenergiasolar.com.br
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="tituloRedeSociais">
                            Siga nossas Redes Sociais:
                        </div>
                        <div class="redesSociais">
                            <a href="http://www.facebook.com/sustentoenergiasolar" target="_blank" title="Facebook"  class="Facebook">
                                <i class="fab fa-fw fa-facebook-f"></i>
                            </a>
                            <a href="http://www.instagram.com/sustentoenergiasolar/" target="_blank" title="Instagram" class="Instagram">
                                <i class="fab fa-fw fa-instagram"></i>
                            </a>
                            <a href="http://www.linkedin.com/company/sustento-energia-solar" target="_blank" title="Linked In" class="Linkedin">
                                <i class="fab fa-fw fa-linkedin-in"></i>
                            </a> 
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
    .contato_bg {
        background-image: url('../assets/contatos/bg-contatos.jpg') ;
        background-position-x: -250px;
        background-position-x: center;
        background-size: cover;
        background-origin: border-box;
        margin-top: 10px;
        min-height: 400px;
        background-repeat: no-repeat;
        padding-top: 40px;
        padding-bottom: 50px;
    }
    .redeSociais_bg {
        background-image: url('../assets/contatos/bg-footer.jpg') ;
        background-size: cover;
        background-position-y: center;
        background-origin: border-box;
        min-height: 250px;
        background-repeat: no-repeat;
    }
    .mapa {
        height: 230px;
        border: #4ea103 2px solid;
    }
    .paddingZero {
        padding: 0 !important;
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
        padding-top: 25px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
        font-weight: 600;
    }
    .sustentaSaoCarlosFinal {
        background-position: left 10px;
        min-height: 48px;
        padding-top: 25px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        font-weight: 600;
    }
    .estiloRuaAquidaban {
        background-position: left 10px;
        padding-left: 80px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
    }
    .estiloRuaRibeirao {
        background-position: left 10px;
        padding-left: 60px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
    }
    .estiloRuaCep {
        background-position: left 10px;
        padding-left: 90px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
    }
    .estiloEmail {
        background-position: left 10px;
        padding-left: 80px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
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
        text-align: left;
        font-weight: 600;
    }
    .iconeLocalizacao {
        border: #4ea103 2px solid;
        color: #4ea103;
        border-radius: 35px;
        padding: 10px;
    }
    .fa-whatsapp {
        color: #4ea103;
        font-size: 1.8em;
    }
    .fa-envelope {
        border: #4ea103 2px solid;
        color: #4ea103;
        border-radius: 30px;
        padding: 10px;
    }
    .tituloRedeSociais {
        background-position: left 10px;
        padding-left: 90px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
    }
    .Facebook:hover {
        color: #fff;
        background-color: #4ea103;
    }
    .Facebook {
        color: #000;
        background-color: #fff;
        border-radius: 30px;
        padding: 5px;
        margin-right: 80px;
    }
    .Instagram:hover {
        color: #fff;
        background-color: #4ea103;
    }
    .Instagram {
        color: #000;
        background-color: #fff;
        border-radius: 30px;
        padding: 5px;
    }
    .Linkedin:hover {
        color: #fff;
        background-color: #4ea103;
    }
    .Linkedin {
        color: #000;
        background-color: #fff;
        border-radius: 30px;
        padding: 5px;
    }
</style>