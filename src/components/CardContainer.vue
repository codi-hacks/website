<template>
  <div class="flex-container">
    <hr/>

    <Card class="flex-item" title="Mini Joker" image_name="mini_joker.png" website="https://github.com/codi-hacks/space-race">
      It's the mini joker!!!!!!!
    </Card>

    <Card class="flex-item" title="Space Race" image_name="space_race.png" website="https://github.com/codi-hacks/space-race">
      Spaceship racer! A spaceship racing game created with the Lua framework <a href="https://love2d.org/">Love2D</a>.
      It is mostly complete, yet it lacks levels!
      If you are interested in helping, please open an issue on our GitHub.
    </Card>
    
    <Card class="flex-item" title="Weather Station" image_name="weather_station.png" website="https://weather.codihacks.org/">
      A <a href="https://github.com/codi-hacks/weather-station">weather station web app</a>.
      It features a physical weather station, an API server written in Rust, and a web app frontend written in Vue.
    </Card>
  </div>
</template>

<script>
import Card from '@/components/Card.vue'
export default {
  name: "Card Container",
  components: {
    Card
  }
}
</script>

<style scoped>
.flex-container {
  display: flex;
  flex-flow: column wrap;
  justify-content: center;
}

.flex-item {
  flex-basis: 100%;
  flex-grow: 1;
  flex-shrink: 0;
  min-height: 20em;

  padding-top: 20px;
  border-top: solid black 2px;
}

.flex-item:last-child {
  padding-bottom: 30px;
}
</style>