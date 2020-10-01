<template>
  <h3>{{ header }}</h3>
  <p v-if="isHidden === false">{{ body }}</p>
  <p @click="hideContent()">Click me!</p>
</template>

<script>
export default {
  name: 'HelloComponent',
  props: {
    header: String,
    body: String
  },
  data() {
    return {
      isHidden: false
    }
  },
  methods: {
    hideContent() {
      this.isHidden = true
    }
  }
}
</script>
