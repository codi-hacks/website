<template>
  <div>
    <img v-if="darkMode" alt="JTCC logo" src="../assets/logoDark.png?">
    <img v-else alt="JTCC logo" src="../assets/logoLight.png?">
    <br>
    <div class="hello">
      <h1>Welcome to the JTCC Programming Club</h1>
      <p>This website is the main project of our club.
        If you would like to learn more, please visit our
        temporary site <a href=http://jtccprogramming.club> here. </a> </p>


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
img {
  width: 40%;
}
p {
  align: left;
}
</style>
