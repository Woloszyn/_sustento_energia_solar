<template>
    <div id="home">
        <div v-if="!menuStick" class="col-12 menu_principal_info">
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
        <div v-else class="menu_opcoes_stick">
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
        },
        changeMenuType() {
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
        background-image: url("../assets/home/banner-2.jpg");
        background-size: cover;
        background-position: center center;
        background-repeat: no-repeat;
        min-height: 98vh;
    }
    .menu_principal_info{
        padding-top: 35px;
        background: linear-gradient(rgba(0, 0, 0, 0.836), transparent) ;
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
    .color_white > a {
        color: white;
    }
    a:hover {
        color: white !important;
    }
    .color_black > a {
        color: black;
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