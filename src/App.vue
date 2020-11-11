<template>
<img v-if="darkMode" alt="JTCC logo" src="./assets/logoDark.png?" width=500>
<img v-else alt="JTCC logo" src="./assets/logoLight.png?" width=500>
<Header msg="Welcome to the JTCC Programming Club" />
<button @click="darkMode = !darkMode" class=buttonLight>TOGGLE DARK/LIGHT IMAGE TEST</button><br>
<darkmode />
</template>

<script>
import Header from './components/Header.vue'
import Darkmode from './components/Darkmode.vue'
export default {
  name: 'App',
  components: {
    Header,
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
