<template>
  <div class="container">
    <div class="switch">
      <ToggleSwitch
        :value="darkMode"
        @update:value="toggleDarkMode"
        />
    </div>
  </div>
</template>

<script>
import ToggleSwitch from './ToggleSwitch'

export default {
  components: {
    ToggleSwitch
  },
  props: {
    darkMode: {
      type: Boolean,
      required: true
    }
  },
  methods: {
    toggleDarkMode(value) {
      this.$emit('update:darkMode', value)
    }
  }

}
</script>

<style scoped>
.container {
  opacity: 90%;
  height: 34px;
  padding: 6px;
  width: 100%;

  /* Fix position on bottom of screen */
  position: fixed;
  top: 100vh;
  left: 0;
  right: 0;
  transform: translateY(-100%);
}

.switch {
  float: left;
}
</style>