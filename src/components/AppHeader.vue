<template>
<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.0/css/all.min.css">
  <div>
    <header>
      <div class="container">
        <div class="content">
          <h1>Codi Hacks</h1>
          <hr>
          <p>Projects</p>
          <hr>
          <p>
            <a href="https://github.com/codi-hacks">
              <i class="fa-brands fa-github" alt="github"></i>
            </a>
          </p>
          <p>
            <a href="https://discord.gg/xKgzfkyaha">
              <i class="fa-brands fa-discord" alt="discord"></i>
            </a>
          </p>
          <hr>
          <p>Navigation</p>
        </div>
      </div>


      <br />
    </header>
      <img v-show="darkMode" alt="JTCC logo" src="../assets/logoDark.png">
      <img v-show="!darkMode" alt="JTCC logo" src="../assets/logoLight.png">
      <br>
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

header {
  backdrop-filter: grayscale(0.25) blur(10px);
  position: sticky;
  top: 0;
}

hr{
  opacity: .25;
}

.container{
  height: 80%;
  padding-right: 16px;
  padding-left: 16px;
}
.content{
  display: flex;
}
</style>
