<template>
  <AppHeader :dark-mode="darkMode" />
  <Projects :dark-mode="darkMode" />
  <AppFooter :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import AppHeader from './AppHeader.vue'
import AppFooter from './AppFooter.vue'
import Projects from './Projects'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
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
