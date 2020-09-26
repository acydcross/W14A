<template>
  <div id="button">
    <button @click="getJokes">Jokes</button>
    <div>
      <button @click="getNormal">Normal Joke</button>
    </div>
    <div>
      <button @click="getLoud">Loud Joke</button>
    </div>
      <button @click="getSnake">Snake Joke</button>
    <div>
    </div>
  </div>
</template>

<script>
export default {
  name: "joke-button",
  methods: {
    getJokes() {
      this.$store.commit("getjokes");
    },
    getLoud() {
      this.$store.commit("loud");
    },
    getSnake() {
      this.$store.commit("snake");
    },
    getNormal() {
      this.$store.commit("normal");
    }
  }
};
</script>

<style scoped></style>
