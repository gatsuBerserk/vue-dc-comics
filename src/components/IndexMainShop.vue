<template>
    <div class="wrapper"> 
        <div class="shop">
            <div class="shop-card" v-for="(element, index) in shopIcon" :key="index"> 
                <a href="#"> 
                    <img class="logos" :src="require(`@/assets/img/${element.shopImg}`)" :alt="element.text"> 
                    {{element.text}}
                </a>
            </div> 
        </div>
    </div>
</template>

<script>
export default { 
    name: "IndexMainShop",
    data : function(){
        return{
            shopIcon : [
                {
                    shopImg: "buy-comics-digital-comics.png", 
                    name: "buy-comics-digital-comics", 
                    text:"Digital Cimics"

                },
                {
                    shopImg: "buy-comics-merchandise.png", 
                    name: "digital comics", 
                    text:"DC merchandise"

                }, 
                {
                    shopImg: "buy-comics-subscriptions.png", 
                    name: "Subscription", 
                    text:"Subscription"

                }, 
                {
                    shopImg: "buy-comics-shop-locator.png", 
                    name: "digital locator", 
                    text:"Comic shop locator"

                }, 
                {
                    shopImg: "buy-dc-power-visa.svg", 
                    name: "digital visa", 
                    text:"Dc power Visa"

                } 

            ]
        }
    }

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

        .shop-card{ 
        height: 100%;
        display: flex; 
        justify-content: space-evenly; 
        align-items: center;
        padding: 0;
                
            img.logos{
            height: 50px; 
            margin-right: 1rem; 
            }
            
            a{ 
                display: flex;
                align-items: center;
                margin-left: 1rem ; 
                text-decoration: none; 
                color: whitesmoke; 
                font-weight:bolder; 
                text-transform: uppercase;
                

                &:hover{
                    color: yellow;
                }
                } 
    }
    } 
    
    

           
     
</style>