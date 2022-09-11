<template>
  <AppHeader :dark-mode="darkMode" />
  <GoogleForm/>
  <AppFooter :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import AppHeader from './AppHeader.vue'
import AppFooter from './AppFooter.vue'
import GoogleForm from './GoogleForm.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
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
