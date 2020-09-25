<template>
  <div>
    <div id="button" @click="getJoke">Get Joke</div>
    <h3>{{ joke }}</h3>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "normal-joke",
  data() {
    return {
      joke: ""
    };
  },
  methods: {
    getJoke: function() {
      axios
        .request({
          url: "https://geek-jokes.sameerkumar.website/api?format=json",
          method: "GET"
        })
        .then(response => {
          this.joke = response.data.joke;
        })
        .catch(error => {
          console.log(error);
        });
    }
  }
};
</script>

<style scoped></style>
