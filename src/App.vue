<template>
  <div id="app">
    <header>
      <nav-bar/>
    </header>
    <main-app/>
    <footer-app/>

    
  </div>
</template>

<script>
import FooterApp from './components/FooterApp.vue';
import MainApp from './components/MainApp.vue';
import NavBar from './components/NavBar.vue' ;
export default {
  name: 'App',
  components: {
    NavBar,
    MainApp,
    FooterApp,
    
  },
  data(){
    return{
      


    }
  },
  
}

</script>

<style lang="scss">
@import  './styles/generals.scss';



</style>
