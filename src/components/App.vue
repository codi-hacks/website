<template>
  <Header :dark-mode="darkMode" />
  <GoogleForm/>
  <Projects />
  <Footer :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import Header from './Header'
import Footer from './Footer'
import GoogleForm from './GoogleForm'
import Projects from './Projects'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    GoogleForm,
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
