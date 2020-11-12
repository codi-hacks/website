<template>
  <div class="container">
    <ToggleSwitch
      :value="darkMode"
      @update:value="toggleDarkMode"
      />
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
  background: black;
  height: 80px;
  padding: 4px;
  width: 100%;
}
</style>
