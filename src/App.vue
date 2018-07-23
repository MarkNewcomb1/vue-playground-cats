<template>
  <div id="app">
    <Header v-bind:cats="cats" v-bind:logCats="logCats"/>
    <img src="./assets/logo.png" v-on:click="logCats">
    <HelloWorld/>
    <h1>HELLOO</h1>
    <p>This is a paragraph</p>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Header from './components/Header'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Header
  },
  data() {
    return {
      cats: ['garfield', 'heathcliff', 'hobbes']
    }
  },
  methods: {
    logCats() {
      console.log(this.cats);
      
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
