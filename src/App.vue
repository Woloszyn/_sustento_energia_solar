<template>
  <div id="app" data-bs-spy="scroll" data-bs-target="#navbar-example2" data-bs-offset="0" class="scrollspy-example" tabindex="0">
    <Menu></Menu>
    <Trabalhos></Trabalhos>
    <OrcamentoOnline></OrcamentoOnline>
    <ComoFunciona></ComoFunciona>
    <ProdutosParceiros></ProdutosParceiros>
    <Contatos></Contatos>
  </div>
</template>

<script>
import Menu from './components/Menu.vue';
import Trabalhos from './components/Trabalhos.vue';
import OrcamentoOnline from './components/OrcamentoOnline';
import ComoFunciona from './components/ComoFunciona';
import ProdutosParceiros from  './components/ProdutosParceiros';
import Contatos from './components/Contatos';

export default {
  name: 'App',
  components: {
    Menu,
    OrcamentoOnline,
    ComoFunciona,
    ProdutosParceiros,
    Contatos,
    Trabalhos
  }
}
</script>

<style>
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
