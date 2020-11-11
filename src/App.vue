<template>
<img v-if="darkMode" alt="JTCC logo" src="./assets/logoDark.png?" style="width:40%">
<img v-else alt="JTCC logo" src="./assets/logoLight.png?" style="width:40%">
<Header msg="Welcome to the JTCC Programming Club" />
<button @click="darkMode = !darkMode" class=buttonLight>TOGGLE DARK/LIGHT IMAGE TEST</button><br>
<darkmode />
<GoogleForm/>
</template>

<script>
import Header from './components/Header.vue'
import GoogleForm from './components/GoogleForm.vue'
import Darkmode from './components/Darkmode.vue'
export default {
  name: 'App',
  components: {
    Header,
    GoogleForm,
    Darkmode
  },
  data() {
    return {
      darkMode: false
    }
  },
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
