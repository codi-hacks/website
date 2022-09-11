<template>
  <Header :dark-mode="darkMode" />
  <Shelf/>
  <Footer :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import Header from './Header'
import Footer from './Footer'
import Shelf from './Shelf'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    Shelf
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
