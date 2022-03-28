<template>
  <div id="app">
    <IndexHeader/> 
    <IndexMainContent/> 
    <IndexMainShop/>
  </div>
</template>

<script>
import IndexHeader from "@/components/IndexHeader.vue" 
import IndexMainContent from "@/components/IndexMainContents.vue" 
import IndexMainShop from "@/components/IndexMainShop.vue"

export default {
  name: 'App',
  components: {
    IndexHeader,
    IndexMainContent, 
    IndexMainShop,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
