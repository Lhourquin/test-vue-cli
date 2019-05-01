<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Index v-for="post in posts" v-bind:key="post" :post="post"/>
  </div>
</template>

<script>
import Index from './components/Index.vue'

export default {
  name: 'app',
  components : {
  Index
  },
  data () {
    return {
      posts : [
      {citation : 'si tu est née en france tu sais que tu est européens ?',
      authors : 'Kenny'},
      {citation : 'fumer c`est mal .. m`voyer',
      authors : 'mr mcKey'}
      ]
    }
      

    }
  }

</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
