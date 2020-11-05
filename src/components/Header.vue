<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>This website is the main project of our club.
      If you would like to learn more, please visit our
      temporary site <a href=http://jtccprogramming.club> here. </a> </p>


  </div>
</template>

<script>
export default {
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
p {
  align: left;
}
</style>
