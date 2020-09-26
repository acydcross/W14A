<template>
    <div>
       <h2>{{ SnakeJoke }}</h2>
    </div>
</template>

<script>
    export default {
        name: "snake-joke",
        computed:{
            SnakeJoke:function(){
                return this.$store.getters.snakeJoke
            }
        }
    }
</script>

<style scoped></style>
