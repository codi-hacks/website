<!--This is the Function and button to toggle Darkmode-->
<script>

export default {
  data() {
    return {
      // Default to no dark mode
      darkMode: false
    }
  },
  methods: {
    toggleDarkmode() {
       this.darkMode = !this.darkMode
       document.body.classList.toggle("dark-mode");
    }

  }
};

</script>

<template>
  <button
    :class="darkMode ? 'buttonDark' : 'buttonLight'"
    id="button"
    @click="toggleDarkmode()">
    Toggle dark mode
  </button>
</template>
