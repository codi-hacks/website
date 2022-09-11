<template>
  <Header :dark-mode="darkMode" />
  <Projects :dark-mode="darkMode"/>
  <Footer :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import Header from './Header'
import Footer from './Footer'
import Projects from './Projects'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Projects
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
