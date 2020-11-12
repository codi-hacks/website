<template>
  <Header :dark-mode="darkMode" />
  <GoogleForm/>
  <Footer :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import Header from './components/Header'
import Footer from './components/Footer'
import GoogleForm from './components/GoogleForm'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    GoogleForm
  },
  data() {
    return {
      darkMode: false
    }
  },
  methods: {
    toggleDarkMode(value) {
      this.darkMode = value
      document.body.classList.toggle('dark-mode')
    }
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
