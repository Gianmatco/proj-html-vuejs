<template>
  <div id="app">
    <header>
      <nav-bar/>

    </header>
    
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue' ;
export default {
  name: 'App',
  components: {
    NavBar,
    
  }
}
</script>

<style lang="scss">
@import  './styles/generals.scss';

</style>
