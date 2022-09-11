<template>
  <div class="main">

    <img :src="require(`@/assets/${image_name}`)"/>

    <div class="body">
      <h2 class="title"> {{ title }} </h2>
      <slot></slot>
      <br/>
    </div>
    <br/>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["title", "image_name", "website"]
}
</script>

<style scoped>
.main {
  background-color: white;
  text-align: left;
}

.body {
  margin: 0 2em;
}

@media screen and (orientation: landscape) {
  .main {
    min-height: 40vh;
  }

  .body {
    float: left;
    max-width: 60vw;
  }

  img {
    float: right;
    height: 40vh;
    max-width: 30vw;
  }
}

@media screen and (orientation: portrait) {
  img {
    max-height: 50vh;
    max-width: 80vw;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }
}
</style>
