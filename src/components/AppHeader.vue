<template>
<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.0/css/all.min.css">

  <div>

    <!--There is a gap above the header. Profoundly unaesthetic, must fix!-->

    <header>
      <div class="container">
        <div class="content">

          <div class="logo-outer">
            <div class="codi-logo"></div>
          </div>

          <h1>Codi Hacks</h1>
          <hr>
          <p></p>
          <hr style="opacity: 0;">

          <!--Dark mode toggle should go here-->

          <hr>

          <!--Icon spacing needs fixing-->
          <p>
            <a href="https://github.com/codi-hacks">
              <i class="fa-brands fa-github fa-xl" alt="github"></i>
            </a>
          </p>
          <p>
            <a href="https://discord.gg/TufC6eRTS7">
              <i class="fa-brands fa-discord fa-xl" alt="discord"></i>
            </a>
          </p>
        </div>
      </div>
      <br />
    </header>

    <!--A variation of the Codi logo must go above h2,
        along with "making it reality" slogan, of course.-->

    <h2>Codi Hacks</h2>
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

h2{
  font-size: 3em;
  background-image:
    linear-gradient(90deg, #0008ff, #ffa600);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}

.container{
  height: 80%;
  padding-right: 16px;
  padding-left: 16px;
}
.content{
  display: flex;
}

.codi-logo {
    background: #3b2c6e;
    width: 50px;
    height: 50px;
    border-radius: 2px;
    position: relative;
    overflow: hidden;
    border: 7px solid #c3c4c4;
    margin: 4px;
}
.codi-logo:before {
    content: "";
    position: absolute;
    background-color: #92c5da;
    width: 10px;
    height: 25px;
    border-radius: 4px;
    top: 10px;
    right: 10px;
}
.codi-logo:after {
    content: "";
    position: absolute;
    background-color: #92c5da;
    width: 10px;
    height: 25px;
    border-radius: 4px;
    top: 10px;
    left: 10px;
}

</style>
