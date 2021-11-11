<template>
  <div id="app">
    <div class="container">
      <Header></Header>
    </div>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "styles/variables";

#app {
}

.container{
  max-width: 1000px;
  margin: auto;
}
</style>
