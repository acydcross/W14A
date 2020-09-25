<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />

  </div>
</template>

<script>
import JokeButton './components/jokebutton.vue'
import LoudJoke './components/loadjoke.vue'
import NormalJoke './components/loadjoke.vue'
import SnakeJoke './components/snakejoke.vue'

export default {
  name: "App",
  components: {
    JokeButton,
    LoudJoke,
    NormalJoke,
    SnakeJoke

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
