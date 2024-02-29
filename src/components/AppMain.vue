<script>
 export default{
    data() {
      return {
        cards: [
          {
            image:'public/img/buy-comics-digital-comics.png' , action:'DIGITAL COMICS'
          },
          {
            image:'/img/buy-comics-merchandise.png' ,action:'DC MERCHANDISE'
          },
          {
            image:'/img/buy-comics-shop-locator.png' , action:'SUBSCRIPTION'
          },
          {
            image:'/img/buy-comics-subscriptions.png' , action:'COMIC SHOP LOCATOR'
          },
          {
            image:'/img/buy-dc-power-visa.svg' , action:'DC POWER VISE'
          },
        ]
      }
    }
 }
</script>

<template>
    <main>
        <div class="container">
            <div class="shopping">

                <div 
                v-for="card in cards"
                class="card" >
                <img :src="card.image" alt="">
                
                <span>{{ card.action }}</span>
    
                </div>
            </div>
           
        </div>
    </main>
</template>

<style>
    main{
        
        background-color: #0282F9;
        
        .shopping{
            display: flex;
            justify-content: center;
            gap: 10px;
            font-size: 10px;
            .card{
                display: flex;
                align-items: center;
                gap: 10px;

                padding: 30px ;
                color: white;
                img{
                    height: 60px;
                }
            }
        }
    }
</style>