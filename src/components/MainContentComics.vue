<template>
  <div class="single-card">
        <img :src="thumb" alt="series">
        <p>{{ price }} {{ series }}</p>
  </div>
</template>

<script>
export default {
    name:"MainContentsComics",
    props: ["thumb", "price", "series"]
}
</script>

<style lang="scss" scoped>
   .single-card{
            width: calc(100% / 6 - (2rem));  
            padding: .5rem; 
            color:whitesmoke; 
        }
</style>