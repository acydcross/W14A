<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <joke-button></joke-button>
  </div>
</template>

<script>
import JokeButton from "./components/jokebutton.vue";
// import LoudJoke from './components/loadjoke.vue'
// import NormalJoke from './components/loadjoke.vue'
// import SnakeJoke from './components/snakejoke.vue'

export default {
  name: "App",
  components: {
    JokeButton
    // LoudJoke,
    // NormalJoke,
    // SnakeJoke

  }
};
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
