<template>
    <div>   
        <h2>{{normalJoke}}</h2>
    </div>
</template>

<script>
    export default {
    name:"normal-joke",
    computed:{
      LoudJoke:function(){
        return this.$store.getters.normalJoke
    }
  }
}
</script>

<style scoped></style>
