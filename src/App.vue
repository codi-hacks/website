<template>
  <img alt="JTCC logo" src="./assets/logo.png">
  <Header msg="Welcome to the JTCC Programming Club"/>
  <GoogleForm/>
</template>

<script>
import Header from './components/Header.vue'
import GoogleForm from './components/GoogleForm.vue'

export default {
  name: 'App',
  components: {
    Header,
    GoogleForm
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
