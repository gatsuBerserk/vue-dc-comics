<template>
  <div class="shop">
      <figure> 
           <!--Appena finito cambiare con una lista e fare un v-for (ci ho pensato dopo mannaggia, meglio tardi che mai)-->
          <div class="shop-card">
            <a href="#"></a> <img class="logos" src="../assets/img/buy-comics-digital-comics.png" alt=" Digitl Store"> 
            <p> Digital Comics</p>
          </div>
          <div class="shop-cards">
            <img class="logos" src="../assets/img/buy-comics-digital-comics.png" alt=" Digitl Store"> 
            <p>Mercandise</p>
          </div>
          <div class="shop-cards">
            <img class="logos" src="../assets/img/buy-comics-digital-comics.png" alt=" Digitl Store"> 
            <p>Sub</p>
          </div>
          <div class="shop-cards">
            <img class="logos" src="../assets/img/buy-comics-digital-comics.png" alt=" Digitl Store"> 
            <p>locator</p>
          </div>
          <div class="shop-cards">
              <img class="logos" src="../assets/img/buy-comics-digital-comics.png" alt=" Digitl Store"> 
              <p>power</p>
          </div>
      </figure>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
    div.shop{
        background-color: rgb(2, 130, 249);  
        height: 100px; 
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        
        figure{ 
            margin: 0;
            display: flex;
            justify-content: space-evenly;  
            align-items: center; 
            
            img.logos{
                height: 50px; 
            }

            div{
                display: flex; 
                justify-content: space-evenly; 
                padding: 4rem; 
                
                p{ 
                margin-left: 1rem ;
                display: inline-block;
                } 
            }
        } 
    } 
</style>