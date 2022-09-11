<template>
    <div>
        <div class="Project">
            <h1 class="projectTitle">Weather Station</h1>
            <p class="projectText">This is our <a href="https://weather.codihacks.org/" target="_blank">weather station</a> web app project! It features a physical weather station, an API server
                written in Rust, and a web app frontend written in Vue.
            </p>
        </div> 
        <div class="Project">
            <h1 class="projectTitle">Space Race</h1>
            <p class="projectText">This is our Spaceship Race project! It is a spaceship game created with the Lua framework <a href="https://love2d.org/" target="_blank">Love2D</a>.
                It lacks levels, so if you are interested in helping, please open an issue on our GitHub.
            </p>
            
        </div>
    </div>
</template>

<script>
export default {
    name: 'Projects',
    props: {
    darkMode: {
      type: Boolean,
      required: true
    }
  }

}
</script>

<style>
        
    .Project{
        display: inline-block;
        background-color: #89c7d0;
        border-radius: 15px;
        color: white;
        height: auto;
        width: 45vw;
        max-width: 97%;
        margin-top: 10vh;
        margin-right: 1vw;
        margin-left: 1vw;
        margin-bottom: 20vh;
    }

    .projectTitle{
        text-align: left;
        margin-left: 1vw;
        margin-top: 35vh;
    }

    .projectText{
        text-align: left;
        margin-left: 1vw;
        font-size: 1.5em;
    }

    .dark-mode .Project {
        background: rgb(238, 238, 62);
        color: #006eff;
    }
</style>