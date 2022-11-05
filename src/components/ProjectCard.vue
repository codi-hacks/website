<template>
  <div class="project">
    <h1 class="project-title">{{ title }}</h1>
    <img class="project-image" :alt="title" :src="image">
    <p class="project-text"><slot /></p>
  </div>
</template>

<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  image: {
    type: String,
    required: true
  }
})
</script>

<style scoped>
.project {
  background-color: #89c7d0;
  border-radius: 15px;
  color: white;
  height: auto;
  width: 46vw;
  margin: 1%;
}

.project-title {
  text-align: center;
}

.project-image {
  border-radius: 1em;
  max-width: 65%;
  max-height: 65%;
}

.project-text {
  text-align: left;
  padding-left: 1vw;
  padding-right: 1vw;
  font-size: 1.5em;
}

.dark-mode .project {
  background: rgb(238, 238, 62);
  color: #006eff;
}

@media screen and (max-width: 725px) {
  .project {
    width: 100%;
    margin-bottom: 2vh;
  }

  .project-text {
    padding-left: 4vw;
    padding-right: 4vw;
  }

  .project-image {
    max-width: 80%;
    max-height: 80%;
  }
}
</style>
