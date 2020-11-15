<template>
  <div>
    <img v-show="darkMode" alt="JTCC logo" src="../assets/logoDark.png">
    <img v-show="!darkMode" alt="JTCC logo" src="../assets/logoLight.png">
    <br />
    <div>
      <h1>Welcome to the JTCC Programming Club</h1>
      <p>This website is the main project of our club.</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    darkMode: {
      type: Boolean,
      required: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@media screen and (min-width: 0px) {
  img {
    width: 100%;
  }
}
@media screen and (min-width: 700px) {
  img {
    width: 75%;
  }
}
@media screen and (min-width: 950px) {
  img {
    width: 50%;
  }
}
</style>
