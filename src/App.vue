<template>
  <div id="app">
    <Menu></Menu>
    <OrcamentoOnline></OrcamentoOnline>
  </div>
</template>

<script>
import Menu from './components/Menu.vue';
import OrcamentoOnline from './components/OrcamentoOnline';

export default {
  name: 'App',
  components: {
    Menu,
    OrcamentoOnline
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
