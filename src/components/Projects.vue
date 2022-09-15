<template>
    <div class="container">
        <div class="project">
            <h1 class="project-title">Weather Station</h1>
            <img class="image1" v-bind:src="image1">
            <p class="project-text">This is our <a href="https://weather.codihacks.org/" target="_blank">weather station</a> web app project! It features a physical weather station, an API server
                written in Rust, and a web app frontend written in Vue.
            </p>
        </div> 
        <div class="project">
            <h1 class="project-title">Space Race</h1>
            <img class="image2" v-bind:src="image2">
            <p class="project-text">This is our Spaceship Race project! It is a spaceship game created with the Lua framework <a href="https://love2d.org/" target="_blank">Love2D</a>.
                It lacks levels, so if you are interested in helping, please open an issue on our GitHub. 
            </p>
        </div>
    </div>
</template>


<script>
    export default{
        name: 'Projects',
        data() {
            return{
               image1: require(`@/assets/weather_station.png`),
               image2: require(`@/assets/space_race.png`) 
            }
        }
    }
</script>


<style scoped>

    .container{
        display: flex;
        flex-wrap: wrap;
        max-width: 100%;
        margin-top: 10vh;
        margin-bottom: 20vh;
        padding: 1%;

    }
        
    .project{
        background-color: #89c7d0;
        border-radius: 15px;
        color: white;
        height: auto;
        min-width: 300px;
        width: 46vw;
        max-width: 97%;
        margin: 1%;
    }

    .project-title{
        text-align: center;
    }

    .image1{
        width: 40%;
        height: auto;
    }
    
    .image2{
        width: 65%;
        height: auto;
    }

    .project-text{
        text-align: left;
        padding-left: 1vw;
        padding-right: 1vw;
        font-size: 1.5em;
    }

    .dark-mode .project {
        background: rgb(238, 238, 62);
        color: #006eff;
    }

    @media screen and (max-width: 600px) {
        .container {
            padding: 5%;
        }

        .project{
            margin: 5%;
        }

        .project-text{
            padding-left: 4vw;
            padding-right: 4vw;
        }
    }
</style>