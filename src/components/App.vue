<template>
  <AppHeader :dark-mode="darkMode" />
  <GoogleForm/>
  <AppFooter :darkMode="darkMode" @update:darkMode="toggleDarkMode" />
</template>

<script>
import AppHeader from '@/components/AppHeader.vue'
import AppFooter from '@/components/AppFooter.vue'
import GoogleForm from '@/components/GoogleForm.vue'

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
