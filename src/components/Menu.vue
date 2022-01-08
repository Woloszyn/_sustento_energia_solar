<template>
    <div id="menu">
        <b-nav>
            <b-nav-item v-for="menu in items_menu" :key="menu.name" :href='menu.link' >
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
                    "link": "#home"
                },
                {
                    "name": "Trabalhos",
                    "link": "#trabalhos"
                },
                {
                    "name": "Orçamento online",
                    "link": "#orcamento_online"
                },
                {
                    "name": "Sobre",
                    "link": "#sobre"
                },
                {
                    "name": "Como funciona?",
                    "link": "#como_funciona"
                },
                {
                    "name": "Produtos e parceiros",
                    "link": "#produtos_e_parceiros"
                },
                {
                    "name": "Contatos",
                    "link": "#contatos"
                },
            ]
        }
    }
}
</script>

<style>

</style>