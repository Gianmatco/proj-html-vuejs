<template>
  <div id="app">
    <header>
      <nav-bar/>
    </header>
    <main-app/>

    
  </div>
</template>

<script>
import MainApp from './components/MainApp.vue';
import NavBar from './components/NavBar.vue' ;
export default {
  name: 'App',
  components: {
    NavBar,
    MainApp,
    
  }
}

</script>

<style lang="scss">
@import  './styles/generals.scss';

</style>
