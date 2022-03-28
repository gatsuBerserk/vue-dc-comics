<template>
  <div> 
      <div class="header">
        <img src="../assets/img/dc-logo.png" alt=" Logo DS Comics">
        <nav>
            <ul>
                <li v-for="(element, index) in manu" :key="index">
                    <a href="#">{{ element.text }}</a>
                </li>
            </ul>
        </nav>
        </div>  
  </div>
</template>

<script>
export default { 
    name : "IndexHeader", 
    data: function(){
        return{ 
            manu :[
                {
                    text : "Characters", 
                    url : "#" 
                },
                {
                    text : "Comics", 
                    url : "#" 
                },
                {
                    text : "Movies", 
                    url : "#" 
                },
                {
                    text : "Tv", 
                    url : "#" 
                },
                {
                    text : "Games", 
                    url : "#" 
                },
                {
                    text : "Collectibles", 
                    url : "#" 
                },
                {
                    text : "Videos", 
                    url : "#" 
                },
                {
                    text : "Fans", 
                    url : "#" 
                },
                {
                    text : "News", 
                    url : "#" 
                },
                {
                    text : "Shop", 
                    url : "#" 
                },

            ]
        
        }
    }

}
</script>

<style lang="scss" scoped>

div.header{
    display: flex; 
    justify-content: space-around; 
    align-items: center; 

    ul{
        display: flex;
    }

    li{
        list-style: none; 
        margin: 1rem; 
        ;

        :hover{
            color: blue;
        }
    } 

    a{
        text-decoration:none; 
        color: black;
        text-transform: uppercase; 

}
}

</style>