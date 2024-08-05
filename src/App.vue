<template>
  <div id="app">
    <HomePage/>
  </div>
</template>

<script>
import HomePage from './components/HomePage.vue';

export default {
  components: {
    HomePage
  }
}
</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  height: 100vh;
}

.bg-black {
  background-color: black !important;
}
</style>