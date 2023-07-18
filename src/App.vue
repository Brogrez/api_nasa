<template>
  <div id="app">

    <ImgNasa />

  </div>
</template>

<script>
import ImgNasa from "./components/ImgNasa.vue"

export default {
  name: 'App',
  components: {
    ImgNasa
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
