<template>
    <div class="wrapper-jumbo">
      <div class="footer-jumbo"> 
            <div class="wrapper">
                <div class="list"> 
                    <h3>Dc comics</h3>
                    <ul> 
                        
                        <li v-for="(element, index) in navFooterComnics" :key="index"> 
                            <a :href=element.url>  {{element.section}} </a>
                            
                            </li>
                    </ul>
                <h3> Shop</h3>
                    <ul>    
                    <li v-for="(element, index) in navFooterShop" :key="index"> 
                        <a :href=element.url>  {{element.section}} </a>
                            
                        </li>
                    </ul>  
                 
                </div>
                   
                <div class="list">
                    <h3>DC</h3> 
                    <ul>
                        <li v-for="(element, index) in navFooterDc" :key="index"> 
                        <a :href=element.url>  {{element.section}} </a> 
                        </li>
                    </ul>
                </div>

                <div class="list">
                    <h3>Sities</h3> 
                    <ul>
                        <li v-for="(element, index) in navFooterSites" :key="index"> 
                        <a :href=element.url>  {{element.section}} </a> 
                        </li>
                    </ul>
                </div>    
            </div>         
          <figure>
              <img src="../assets/img/dc-logo-bg.png" alt=" DC Logo">
          </figure> 
      </div> 
        <section class="social">  
            <div class="sign-social"> 
                <button>Sing-up now!</button>
                <div class="social" >
                    <h4>Follow us</h4> 
                    <!-- non funzionanano png -->
                    <!-- <figure v-for="(element, index) in socials" :key="index">
                        <img :src="`../src/img` + element.socialImg" :alt="element.text"> 
                    </figure>  --> 
                    <figure>
                        <img src="../assets/img/footer-facebook.png" alt=""> 
                        <img src="../assets/img/footer-periscope.png" alt=""> 
                        <img src="../assets/img/footer-pinterest.png" alt=""> 
                        <img src="../assets/img/footer-twitter.png" alt=""> 
                        <img src="../assets/img/footer-youtube.png" alt=""> 
                    </figure> 
                </div>
            </div> 
        </section>
    </div>
</template>

<script>
export default {
    name : "IndexFooter",
    data : function(){
        return{ 
            navFooterComnics:[
                {
                    section:"Characters", 
                    url : "#"
                }, 
                {
                    section:"Commics", 
                    url : "#"
                }, 
                {
                    section:"Movies", 
                    url : "#"
                }, 
                {
                    section:"Tv", 
                    url : "#"
                }, 
                {
                    section:"Games", 
                    url : "#"
                }, 
                {
                    section:"Video", 
                    url : "#"
                }, 
                {
                    section:"News", 
                    url : "#"
                }, 
                
            ], 
             navFooterShop:[
                {
                    section:"Shop Dc", 
                    url : "#"
                }, 
                {
                    section:"Shop Dc Collectibles", 
                    url : "#"
                } 
            ], 
            navFooterDc:[
                {
                    section:"Terms Of Use", 
                    url : "#"
                }, 
                {
                    section:"Privacy policy (New)", 
                    url : "#"
                },
                {
                    section:"Ad Choices", 
                    url : "#"
                }, 
                {
                    section:"Advertising", 
                    url : "#"
                }, 
                {
                    section:"Jobs", 
                    url : "#"
                }, 
                {
                    section:"Subscriptioins", 
                    url : "#"
                },  
                {
                    section:"Talent Workshops", 
                    url : "#"
                }, 
                {
                    section:"CPSC Certificates", 
                    url : "#"
                }, 
                {
                    section:"Ratings", 
                    url : "#"
                }, 
                {
                    section:"Shop Helps", 
                    url : "#"
                }, 
                {
                    section:"Contct US", 
                    url : "#"
                }, 

            ], 
            navFooterSites:[
                {
                    section:"DC", 
                    url : "#"
                }, 
                {
                    section:"MAD Magazine", 
                    url : "#"
                },
                {
                    section:"DS Kids", 
                    url : "#"
                }, 
                {
                    section:"DC Unicers", 
                    url : "#"
                }, 
                {
                    section:"DC power Visa", 
                    url : "#"
                },  
            ],       

            socials : [
                { 
                    socialImg : "footer-facebook.png", 
                    text: "Facebook"
                },
                { 
                    socialImg : "footer-periscope.png", 
                    text: "Periscope"
                }, 
                 { 
                    socialImg : "footer-pinterest", 
                    text: "Pinterest"
                }, 
                 { 
                    socialImg : "footer-twitter.png", 
                    text: "Twitter"
                },  { 
                    socialImg : "footer-youtube.png", 
                    text: "YouTube"
                }  

            ]
        }
    }
}
</script>

<style lang="scss" scoped> 
@import "../assets/scss/style.scss";
 div.wrapper-jumbo{
      background: url("../assets/img/footer-bg.jpg") no-repeat;
      background-size: 100%; 

        div.footer-jumbo{ 
        @include container; 
        overflow: hidden;
        height: 400px;  
        
        .wrapper{
            display: flex;
            justify-content: space-around;
        }

        div.list{
            padding-right: 1.8rem;
        }

        h3{
            text-align: left;
            color: white;
            margin-bottom: .5rem;
        }

        ul{
            padding: 0;
        }

        li{
            text-align: left;
            list-style: none;
            
        }

        a{
            color: yellow;
            text-decoration: none;
        }

        figure img{ 
            height: 600px; 
        }
    }  
    section.social{
        background-color: rgb(48, 48, 48); 

        div.sign-social{ 
        @include container;
        button{ 
            background-color: transparent; 
            color: white;
            text-transform:uppercase; 
            height: 30px; 
            width: 150px;
            border: 2px solid $primaryColor; 
        } 

        div.social{ 
            display: flex;
            
            h4{
            text-transform: uppercase;
            color: $primaryColor ;
        } 

            img{
                margin-left: 1rem;
            }
        } 
            
    }

    }

 }
    

    

</style>