<template>
  <div class="form-container">
    <p>If you are interested in joining, please fill out your contact info in the form below and our club president will get back to you.</p>
    <br />
    <p>Programmers of <b>all</b> skill levels welcome!</p>
    <iframe
      frameborder="0"
      height="1050"
      marginheight="0"
      marginwidth="0"
      src="https://docs.google.com/forms/d/e/1FAIpQLSd1__tmuMPAw5j3uKujuDw1ibA2vSBYvu3Ww50eGQJIj6EejA/viewform?embedded=true"
      width="100%">
      Sign-up form is loading...
    </iframe>
  </div>
</template>

<style scoped>
iframe {
  max-width: 100%;
  min-width: 200px;
  max-height: auto;
}

.form-container, .form-header, p {
  margin: auto;
}

@media screen and (min-width: 0px) {
  .form-container, p {
    max-width: 100%;
  }
}
@media screen and (min-width: 700px) {
  .form-container, p {
    max-width: 85%;
  }
}
@media screen and (min-width: 950px) {
  .form-container, p {
    max-width: 75%;
  }
}
</style>
