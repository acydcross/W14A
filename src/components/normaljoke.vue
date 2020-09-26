<template>
    <div>   
        <h2>{{normalJoke}}</h2>
    </div>
</template>

<script>
    export default {
        name: "normal-joke",
        computed: {
           normalJoke: function(){
               return this.$store.state.joke
           }
        },
    }
</script>

<style scoped></style>
