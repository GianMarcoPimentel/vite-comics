<script>
import CoverItem from './CoverItem.vue';


export default{
        nome:'AppHeader',

        components : {
        CoverItem,
    },

        data(){
            return {
              covers: [
  {
        humb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
        rice: "$19.99",
        series: "Action Comics",
        type: "comic book",
  },
  {
        humb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
        rice: "$3.99",
        series: "American Vampire 1976",
        type: "comic book",
  },
  {
        humb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
        rice: "$16.99",
        series: "Aquaman",
         type: "graphic novel",
  },
  {
        humb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
        rice: "$2.99",
        series: "Batgirl",
        type: "comic book",
  },
    {
        humb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
        rice: "$3.99",
        series: "Batman",
        type: "comic book",
  },
  {
        humb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
        rice: "$2.99",
        series: "Batman Beyond",
        type: "comic book",
  },
    {
        humb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
        rice: "$3.99",
        series: "Batman/Superman",
        type: "comic book",
  },
  {
        humb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
        rice: "$4.99",
        series: "Batman/Superman Annual",
        type: "comic book",
  },
    {
        humb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
        rice: "$5.99",
        series: "Batman: The Joker War Zone",
        type: "comic book",
  },
  {
        humb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
        rice: "$6.99",
        series: "Batman: Three Jokers",
        type: "comic book",
  },
    {
        humb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
        rice: "$4.99",
        series: "Batman: White Knight Presents: Harley Quinn",
        type: "comic book",
  },
  {
        humb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
        rice: "$16.99",
        series: "Catwoman",
        type: "graphic novel",
  },
]  
            }
        }
    }
</script>

<template>
    <header>
        <img src="/img/jumbotron.jpg" alt="">
        <div class="container">
            <h2>current series</h2>
    
                <div class="covers-list">
                    <!-- <div 
                    v-for="cover in covers" 
                    class="cover"
                    >
                        <img src="" alt="">
                        <h4>Catwoman</h4>
                    </div> -->
                    <CoverItem
                    v-for="currentCover in covers"
                    :coverSerie="currentCover.series"
                    :coverImage="currentCover.humb"
                    ></CoverItem>
                    
                </div>
                <div class="bottone">
                    <button class="btn">LOAD MORE</button>
                </div>
                
        </div>
       
    </header>
</template>

<style >
header{
    background-color: #1C1C1C;
    color: white;
    img{
     height: 410px;
     width: 100%;
     object-fit: cover;
     object-position: top;
    }
    .covers-list{

        display: flex;
        flex-flow: wrap;
        gap: 25px;

        padding: 25px;

    }
    .cover{

        width: calc(100% / 6 - ( 25px / 6 * 5));
        
        img{
            width: 100%;
            height: 185px;
        }
        
    }
    .bottone{
        display: flex;
        justify-content: center;
        padding: 25px 0px;
    }
    .btn{
        background-color: #0282F9;
        border: #0282F9;
        color: white;
        padding: 10px 50px;
        
    }
}
</style>