<script>
    export default {
       nome: 'AppFoterTop',

       data() {
        return {
            linkList: [
                    {
                        title: 'dc comics',
                        links:['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                    },
                    {
                        title: 'shop',
                        links:['Shop DC', 'Shop DC Collectibles']
                    },
                    {
                        title: 'dc',
                        links:['Terms of Use', 'Privacy Policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshop', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                    },
                    {
                        title: 'sites',
                        links:['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                    },
                ],
        }
       }
    }
</script>

<template>
<div class="footer-top">
    <div class="container">
        <div class="lists">
    
    <div v-for="currentLinkList in linkList" class="link-list">
        <h4>{{ currentLinkList.title }}</h4>
        <ul>
            <li v-for="currentLink in currentLinkList.links">{{ currentLink }}</li>
            
        </ul>
    </div>
    
</div>


        <div class="logo">
            <img src="/img/dc-logo-bg.png" alt="">
        </div>
    </div>
</div>
</template>

<style>
ul {
    list-style: none;

    padding: 0;

    li{
        color: #ffffff40;
    }

}
.footer-top{
    height: 370px;
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;

        overflow: hidden;
    }
    .lists{
        display: flex;
        flex-flow: column wrap;
        align-content: flex-start;
        gap: 25px 30px;
        height: 100%;

        padding: 20px 0;

        h4{
            text-transform: uppercase;
            font-size: 1.2em;
            font-family: 'Barlow Condensed', sans-serif;

            color: white;
            margin-bottom: 20px;
        }
        ul {
        color: #ccc;
        font-size: .9em;
    }
    }
   
    .logo{
        z-index: 999;
        
        object-fit: contain;
        object-position: center;
    }
    
}

</style>
