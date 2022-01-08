<template>
    <div id="menu">
        <a href="">
            <img src="../assets/home/logo.png" alt="" srcset="">
        </a>
        <b-nav v-if="!menuStick" pills align="center">
           <b-nav-item v-for="menu in items_menu" :active="menu.active" :key="menu.name" :href='menu.link' @click="changeActive(menu)">
                {{menu.name}}
            </b-nav-item>
        </b-nav>
        <b-nav v-else pills align="center">
           <b-nav-item v-for="menu in items_menu" :active="menu.active" :key="menu.name" :href='menu.link' @click="changeActive(menu)">
                {{menu.name}}
            </b-nav-item>
        </b-nav>
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
    methods: {
        changeActive(menu) {
            this.items_menu.forEach((item) => {
                if(item.name === menu.name) {
                    item.active = true;
                } else {
                    item.active = false;
                }
            });
        }
    }
}
</script>

<style>
    #menu{
        background-image: url("../assets/home/banner-2.jpg");
        background-size: 100%;
        background-repeat: no-repeat;
        min-height: 100vh;
    }
    .nav-link {
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