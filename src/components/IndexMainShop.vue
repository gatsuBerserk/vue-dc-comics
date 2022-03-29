<template>
    <div class="wrapper"> 
        <div class="shop">
            <!--Appena finito cambiare con una lista e fare un v-for (ci ho pensato dopo mannaggia, meglio tardi che mai)--> 
            <!-- non funzionano png -->
            <!-- <div class="shop-card" v-for="(element, index) in shopIcon" :key="index">
                <img class="logos" :src="`../assets/img/` + element.shopImg" :alt="element.text"> 
                <p> {{element.text}} </p>
            </div> --> 
            <div class="shop-cards">
                <img class="logos" src="../assets/img/buy-comics-digital-comics.png" alt="Digital Store"> 
                <p> Digital Store</p> 
            </div>
            <div class="shop-cards">
                <img class="logos" src="../assets/img/buy-comics-merchandise.png" alt=" Digitl Store"> 
                <p>Mercandise</p>
            </div>
            <div class="shop-cards">
                <img class="logos" src="../assets/img/buy-comics-shop-locator.png" alt=" Digitl Store"> 
                <p>Sub</p>
            </div>
            <div class="shop-cards">
                <img class="logos" src="../assets/img/buy-comics-subscriptions.png" alt=" Digitl Store"> 
                <p>locator</p>
            </div>
            <div class="shop-cards">
                <img class="logos" src="../assets/img/buy-dc-power-visa.svg" alt=" Digitl Store"> 
                <a href="#"><p>power</p></a>
            </div> 
        </div>
    </div>
</template>

<script>
export default { 
    name: "IndexMainShop",
    // data : function(){
    //     return{
    //         shopIcon : [
    //             {
    //                 shopImg: "buy-comics-digital-comics.png", 
    //                 name: "buy-comics-digital-comics", 
    //                 text:"Digital Cimics"

    //             },
    //             {
    //                 shopImg: "buy-comics-merchandise.png", 
    //                 name: "digital comics", 
    //                 text:"DC merchandise"

    //             }, 
    //             {
    //                 shopImg: "buy-comics-subscriptions.png", 
    //                 name: "Subscription", 
    //                 text:"Subscription"

    //             }, 
    //             {
    //                 shopImg: "buy-comics-digital-locator.png", 
    //                 name: "digital locator", 
    //                 text:"Comic shop locator"

    //             }, 
    //             {
    //                 shopImg: "buy-dc-power-visa.png", 
    //                 name: "digital visa", 
    //                 text:"Dc power Visa"

    //             } 

    //         ]
    //     }
    // }

}
</script>

<style lang="scss" scoped> 
@import "../assets/scss/style.scss"; 
    div.wrapper{
         background-color: $primaryColor;
    }
    div.shop{ 
        @include container;
        height: 100px; 
         
        // display: flex;
        // align-items: center;
        // justify-content: space-evenly;
             
            
           
    } 
    
    .shop-cards{ 
        height: 100px;
        display: flex; 
        justify-content: space-evenly; 
        align-items: center;
        padding: 0; 
                
            img.logos{
            height: 50px; 
            }
            
            p{ 
                margin-left: 1rem ;
                display: inline-block;
                } 
    }

           
     
</style>