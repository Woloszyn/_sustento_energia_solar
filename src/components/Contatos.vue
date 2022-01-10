<template>
    <div id="contatos">
        <div class="col-12"> 
            <div class="row contato_bg">
                <div class="col-12">
                    <div class="tituloContato">Contato</div>
                </div>
                <div class="col-12">
                    <div class="row estiloEnderecos">
                        <div class="col-2"></div>
                        <div class="col-3"> 
                            <address class="enderecos_address">
                                <span class="titulo_endereco">
                                    <b>Sustento Energia - São Carlos</b>
                                </span>
                                <br>
                                <i>Rua Aquidaban, 1 Centro, São Carlos/SP - CEP 13.560-120 </i>
                            </address>
                            <address class="enderecos_address">
                                <span class="titulo_endereco">
                                    <b>Sustento Energia - Catanduva</b>
                                </span>
                                <br> Rua Ribeirão Preto, 411 <br> Vila Rodrigues, Catanduva/SP <br> - CEP 15.801-340
                            </address>
                        </div>
                        <div class="col-2">
                            <center>
                                    <a href="https://web.whatsapp.com/send?phone=5517981907484&amp;text=Olá!" target="_blank" class="whatsApp"><i class="fab fa-whatsapp icones"></i> (17) 98190-7484</a>
                            </center>
                        </div>
                        <div class="col-3">
                            <i class="fas fa-envelope icones bordaIcones"></i> contato@sustentoenergiasolar.com.br
                        </div>
                        <div class="col-2">
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
                        <img src="../assets/contatos/logo-sustento.png" class="imagemSustento">
                    </div>
                    <div class="col-4 enderecosRodape">
                        <div class="row">
                            <div class="col-12">
                                <center>
                                    <address>
                                        <b>Sustento Energia - São Carlos</b>
                                        <br>
                                        Rua Aquidaban, 1 Centro - São Carlos/SP 
                                    </address>
                                    <address>
                                        <b>Sustento Energia - Catanduva</b>
                                        <br>
                                        Rua Ribeirão Preto, 411 Vila Rodrigues - Catanduva/SP
                                    </address>
                                </center>
                            </div>
                        </div>
                        <div class="row row_sem_espaco_topo">
                            <center>
                                <div>
                                    <a href="https://web.whatsapp.com/send?phone=5517981907484&amp;text=Olá!" target="_blank" class="whatsApp" style=" text-decoration: underline;">
                                        Whatsapp: (17) 98190-7484
                                    </a>
                                </div>
                                <div>
                                    E-mail: contato@sustentoenergiasolar.com.br
                                </div>
                            </center>
                        </div>
                    </div>
                    <div class="col-4">
                        <div class="tituloRedeSociais">
                            Siga nossas Redes Sociais:
                        </div>
                        <div class="linha_flex">
                            <div class="coluna-flex">
                                <div class="circuloRedeSocial">
                                    <a href="http://www.facebook.com/sustentoenergiasolar" target="_blank" title="Facebook"  class="Facebook">
                                        <i class="fab fa-fw fa-facebook-f"></i>
                                    </a>
                                </div>
                            </div>
                            <div class="coluna-flex">
                                <div class="circuloRedeSocial">
                                    <a href="http://www.instagram.com/sustentoenergiasolar/" target="_blank" title="Instagram" class="Instagram">
                                        <i class="fab fa-fw fa-instagram"></i>
                                    </a>
                                </div>
                            </div>
                            <div class="coluna-flex">
                                <div class="circuloRedeSocial">
                                    <a href="http://www.linkedin.com/company/sustento-energia-solar" target="_blank" title="Linked In" class="Linkedin">
                                        <i class="fab fa-fw fa-linkedin-in"></i>
                                    </a> 
                                </div>
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
    .estiloEnderecos {
        min-height: 48px;
        font-size: 15px;
        color: #fff;
    }
    .enderecosRodape {
        background-position: left 10px;
        min-height: 48px;
        font-size: 14px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
        padding-top: 60px;
        font-family: 'Montserrat', sans-serif;
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
        margin-left: 30px;
    }
    .tituloRedeSociais {
        background-position: left 10px;
        padding-left: 90px;
        font-size: 15px;
        color: #fff;
        font-style: italic;
        font-weight: lighter;
        text-align: left;
        margin-top: 80px;
    }
    .circuloRedeSocial:hover {
        color: #fff;
        background-color: #4ea103;
    }
    .circuloRedeSocial > a {
        color: #000;
    }
    .enderecos_address {
        text-align: left;
    }
    .enderecos_address::before {
        font-family: 'Font Awesome 5 Free';
        font-weight: 900;
        border: #4ea103 2px solid;
        border-radius: 50%;
        color: #4ea103;
        font-size: 1.2em;
        position: relative;
        left: -75%;
        padding: 4px;
        content: '\f3c5';
    }
    .circuloRedeSocial {
        background-color: #fff;
        border-radius: 80%;
        max-width: 100%;
    }
    .linha_flex {
        width: 20%;
        display: flex;
        margin-left: 30%;
        flex-direction: row;
    }
    .coluna-flex {
        width: 100%;
        margin-left: 5px;
    }
    .imagemSustento {
        margin-top: 80px;
        margin-left: 150px;
    }
    .icones {
        color: #4ea103;
        font-size: 1.5em;
    }
    .titulo_endereco {
        float: left;
    }
    .bordaIcones{
        border: #4ea103 2px solid;
        border-radius: 50%;
        padding: 4px;
    }
</style>