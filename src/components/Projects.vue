<template>
  <div class="container">
    <ProjectCard title="Weather Station" image="../assets/weather_station.png">
      This is our <a href="https://weather.codihacks.org/" target="_blank">weather station</a> web app project!
      It features a physical weather station, an API server written in Rust, and a web app frontend written in Vue.

    </ProjectCard>
    <ProjectCard title="Space Race" image="../assets/space_race.png">
      This is our Spaceship Race project! It is a spaceship game created with the Lua framework <a href="https://love2d.org/" target="_blank">Love2D</a>.
          It lacks levels, so if you are interested in helping, please open an issue on our GitHub.
    </ProjectCard>
	</div>
</template>

<script setup>
import ProjectCard from './ProjectCard.vue'
</script>

<style scoped>
.container {
  display: flex;
  flex-wrap: wrap;
  max-width: 100%;
  margin-top: 1em;
  margin-bottom: 3em;
  padding: 1%;
}
</style>
