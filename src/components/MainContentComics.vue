<template>
  <div class="single-card">
        <img :src="comicObject.thumb" alt="comicObject.series">
        <p>{{ comicObject.price }} {{ comicObject.series }}</p>
  </div>
</template>

<script>
export default {
    name:"MainContentsComics",
    props: ["comicObject"],
}
</script>

<style lang="scss" scoped>
   .single-card{
            width: calc(100% / 6 - (2rem));  
            padding: .5rem; 
            color:whitesmoke; 
            
            p{
              height: 10px;
            }
        }
</style>