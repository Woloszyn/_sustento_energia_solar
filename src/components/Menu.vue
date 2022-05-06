<template>
    <div id="home">
        <div v-if="menuMobile" class="col-12 menu_mobile">
            <div class="col-1">
                <transition v-if="!show_menus_mobile" name="fade">
                    <button @click="show_menus_mobile = !show_menus_mobile" class="btn btn_mobile"> <i class="fa fa-bars"></i> </button>
                </transition>
                <transition v-else name="fade">
                    <button @click="show_menus_mobile = !show_menus_mobile" class="btn btn_mobile"> <i class="fa fa-times"></i> </button>
                </transition>
            </div>
            <div class="col-11">
                <a v-if="!menuStick" href="">
                    <img src="../assets/home/logo.png" alt="" srcset="">
                </a>
            </div>
            <div class="row" v-if="show_menus_mobile">
                <div class="col-12">
                    <b-list-group>
                        <b-list-group-item class="options_menu_mobile" v-for="menu in items_menu" :active="menu.active" :key="menu.name" :href='menu.link' @click="changeActive(menu)">
                            {{menu.name}}
                        </b-list-group-item>    
                    </b-list-group>
                </div>
            </div>
        </div>
        <div v-else-if="!menuStick && !menuMobile" class="col-12 menu_principal_info">
            <a href="">
                <img src="../assets/home/logo.png" alt="" srcset="">
            </a>
            <hr class="sem_background">
            <b-nav pills align="center">
                <b-nav-item class="color_white" v-for="menu in items_menu" :active="menu.active" :key="menu.name" :href='menu.link' @click="changeActive(menu)">
                    {{menu.name}}
                </b-nav-item>
            </b-nav>
        </div>
        <div v-else-if="menuStick && !menuMobile" class="menu_opcoes_stick">
            <nav class="navbar navbar-light bg-light">
                <div class="container-fluid justify-content-center">
                    <a class="navbar-brand" href="#">
                        <img src="../assets/home/logo-in-black.png" alt="" width="200" height="60" class="d-inline-block align-text-top">
                    </a>
                    <b-nav pills align="center">
                        <b-nav-item v-for="menu in items_menu" class="color_black" :active="menu.active" :key="menu.name" :href='menu.link' @click="changeActive(menu)">
                            {{menu.name}}
                        </b-nav-item>
                    </b-nav>
                </div>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    data: () => {
        return {
            items_menu: [
                {
                    "name": "Home",
                    "link": "#home",
                    "active": true
                },
                {
                    "name": "Trabalhos",
                    "link": "#trabalhos",
                    "active": false
                },
                {
                    "name": "Orçamento online",
                    "link": "#orcamento_online",
                    "active": false
                },
                {
                    "name": "Sobre",
                    "link": "#sobre",
                    "active": false
                },
                {
                    "name": "Como funciona?",
                    "link": "#como_funciona",
                    "active": false
                },
                {
                    "name": "Produtos e parceiros",
                    "link": "#produtos_e_parceiros",
                    "active": false
                },
                {
                    "name": "Contatos",
                    "link": "#contatos",
                    "active": false
                },
            ],
            menuStick: false,
            menuMobile: false,
            show_menus_mobile: false,
        }
    },
    mounted() {
        setInterval(this.changeMenuType, 200);
    },
    methods: {
        changeActive(menu) {
            this.items_menu.forEach((item) => {
                if(item.name === menu.name) {
                    item.active = true;
                } else {
                    item.active = false;
                }
            });
            this.show_menus_mobile = false;
        },
        changeMenuType() {
            if(document.scrollingElement.scrollWidth < 980) {
                this.menuMobile = true
            } else {
                this.menuMobile = false
            }
            if(document.scrollingElement.scrollTop >= 231) {
                this.menuStick = true;
            } else {
                this.menuStick = false;
            }
        }
    }
}
</script>

<style>
    #home{
        background-image: linear-gradient(rgba(0, 0, 0, 0.61), rgba(0, 0, 0, 0.007)), url("../assets/home/banner-2.jpg");
        background-size: cover;
        background-position: center center;
        background-repeat: no-repeat;
        min-height: 98vh;
    }
    .menu_mobile {
        position: fixed;
        z-index: 999999;
        top: 0;
        width: 100%;
        background-color: rgba(0, 0, 0, 0.527) !important;
    }
    .menu_principal_info{
        padding-top: 35px;
        background: linear-gradient(rgba(0, 0, 0, 0.836), rgba(0, 0, 0, 0.082)) ;
    }
    .sem_background{
        background-color: transparent;
    }
    .menu_opcoes_stick{
        position: fixed;
        z-index: 999999;
        top: 0;
        width: 100%;
        background-color: white;
    }
    .btn_mobile {
        color: white !important;
        font-size: 2rem !important;
    }

    .fade-enter-active, .fade-leave-active {
    transition: opacity .5s;
    }
    .fade-enter, .fade-leave-to /* .fade-leave-active em versões anteriores a 2.1.8 */ {
    opacity: 0;
    }

    .color_white > a {
        color: white;
    }
    a:hover {
        color: white !important;
    }
    .color_black > a {
        color: black;
    }
    a.active.options_menu_mobile {
        background: white !important;
        background-color: rgb(3, 151, 23) !important;
    }
    .options_menu_mobile {
        background-color: rgba(0, 0, 0, 0.527) !important;
        color: white !important;
    }
    .nav-link:hover {
        background: linear-gradient(90deg, rgba(54,127,70,0) 0%,
                                     rgba(54,127,70,0.75) 10%,
                                     rgba(54,127,70,0.95) 15%,
                                     rgba(54,127,70,1) 20%,
                                     rgba(54,127,70,1) 80%,
                                     rgba(54,127,70,0.95) 85%,
                                     rgba(54,127,70,0.75) 90%,
                                     rgba(54,127,70,0) 100%) !important;
    }
    .active {
        color: white !important;
        background: linear-gradient(90deg, rgba(54,127,70,0) 0%,
                                     rgba(54,127,70,0.75) 10%,
                                     rgba(54,127,70,0.95) 15%,
                                     rgba(54,127,70,1) 20%,
                                     rgba(54,127,70,1) 80%,
                                     rgba(54,127,70,0.95) 85%,
                                     rgba(54,127,70,0.75) 90%,
                                     rgba(54,127,70,0) 100%) !important;
    }
</style>