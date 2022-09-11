<template>
  <Header :dark-mode="darkMode" />
  <CardContainer/>
  <Footer :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import Header from './Header'
import Footer from './Footer'
import CardContainer from './CardContainer'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    CardContainer
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
