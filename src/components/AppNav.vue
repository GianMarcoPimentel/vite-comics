<script>
    export default{
        nome:'AppNav',
        data(){
            return {
                links :[
                    "characters",
                    "comics",
                    "movies",
                    "tv",
                    "games",
                    "Collectibles",
                    "videos",
                    "fans",
                    "news",
                    "shop",
                ]
            }
        }
    }
</script>

<template>
    <div class="container">
    <nav>
            <img src="/img/dc-logo.png" alt="Logo DC">
            <ul>
                <li v-for="currentLink in links">
                    <a href="">{{currentLink}}</a>
                </li>
               
            </ul>
        </nav>
    </div> 
</template>

<style>
 nav{
    height: 120px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0px;
    img{
        height: 100%;;
    }
    ul{
        display: flex;
        gap: 20px;
        
        list-style-type: none;
        a{
            text-decoration: none;
            color: black;
            text-transform: uppercase;
            &:hover{
                color: blue;
            }
        }
        li:hover{
           
           border-bottom: 5px blue solid;
        }
    }
}

 
</style>