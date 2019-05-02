<template>
  <div id="app">
  <NavBar/>
  <Header/>
  <Footer/>
  <Main/>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import Main from './components/Main.vue'

export default {
  name: 'app',
  components : {
    NavBar,
    Header,
    Main,
    Footer
  }
 }

</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display : grid;
  grid-template-areas: "nav header"
                       "nav main"
                       "nav footer";
  color: #2c3e50;
}
</style>
