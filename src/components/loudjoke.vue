<template>
    <div>
           <h2>{{ LoudJoke }}</h2>
    </div>
</template>

<script>
    export default {
    name:"loud-joke",
           computed:{
            LoudJoke:function(){
                return this.$store.getters.loudJoke
            }
        }
    }
</script>

<style scoped></style>
