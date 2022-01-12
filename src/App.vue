<template>
  <div id="app" data-bs-spy="scroll" data-bs-target="#navbar-example2" data-bs-offset="0" class="scrollspy-example" tabindex="0">
    <Menu></Menu>
    <Trabalhos></Trabalhos>
    <OrcamentoOnline></OrcamentoOnline>
    <Sobre></Sobre>
    <ComoFunciona></ComoFunciona>
    <ProdutosParceiros></ProdutosParceiros>
    <Contatos></Contatos>
  </div>
</template>

<script>
import Menu from './components/Menu.vue';
import Trabalhos from './components/Trabalhos';
import OrcamentoOnline from './components/OrcamentoOnline';
import ComoFunciona from './components/ComoFunciona';
import ProdutosParceiros from  './components/ProdutosParceiros';
import Contatos from './components/Contatos';
import Sobre from './components/Sobre';

export default {
  name: 'App',
  components: {
    Menu,
    OrcamentoOnline,
    Sobre,
    ComoFunciona,
    ProdutosParceiros,
    Contatos,
    Trabalhos,
  }
}
</script>

,
    Rodape<style>
body { 
  overflow-x: hidden;
}
*::-webkit-scrollbar{
  width: 5px;
}
*::-webkit-scrollbar-thumb{
  background: green;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
