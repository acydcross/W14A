<template>
    <div>
        <h2 @click="getJoke">{{ joke }}</h2>
    </div>
</template>

<script>
import axios from "axios"

    export default {
        name: "geek-joke",
        data() {
            return {
                joke: "Click Me!"
            }
        },
        methods: {
            getJoke: function() {
                axios.request( {
                    url: "https://geek-jokes.sameerkumar.website/api?format=json",
                    method: "GET"
                }).then((response) => {
                    this.joke = response.data.joke
                }).catch((error) => {
                    console.log(error)
                })
            }
        },
    }
</script>

<style scoped>

</style>