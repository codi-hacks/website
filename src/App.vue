<template>
  <img alt="JTCC logo" src="./assets/logo.png">
  <Header msg="Welcome to the JTCC Programming Club"/>
<darkmode/>
</template>

<script>
import Header from './components/Header.vue'
import Darkmode from './components/Darkmode.vue'
export default {
  name: 'App',
  components: {
    Header,
    Darkmode
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;

  margin-top: 60px;
}
</style>
