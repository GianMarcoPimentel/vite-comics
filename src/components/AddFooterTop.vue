<script>
    export default {
       nome: 'AppFoterTop',

       data() {
        return {
            programs:[ 
                    "Characters",
                    "Comics",
                    "Movies",
                    "Tv",
                    "Games",
                    "Collectibles",
                    "Videos",
                    "Fans",
                    "News",
                    "Shop",
            ],
            policies : [
                
            ],
            sites:[
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa",
            ],
            shops:[
                "Shop DC",
                "Shop DC collectibles"
            ]
        }
       }
    }
</script>

<template>
<div class="footer-top">
    <div class="container">
        <div class="lists">
            <div id="first-list">
                <ul>
                    <span id="title-list">DC COMICS</span>
                    <li v-for="list in programs">
                    {{ list }}
                    </li>
                </ul>
            </div>
            
            <div id="second-list">
                <span id="title-list">DC COMICS</span>
                    <li v-for="policy in policies">
                    {{ policy }}
                    </li>
            </div>

            <div id="third-list">
                <span id="title-list">DC COMICS</span>
                    <li v-for="site in sites">
                    {{ site }}
                    </li>
            </div>
            <div id="fourth-list">
                <span id="title-list">DC COMICS</span>
                    <li v-for="shop in shops">
                    {{ shop }}
                    </li>
            </div>
        </div>

        <div class="logo">
            <img src="/img/dc-logo-bg.png" alt="">
        </div>
    </div>
</div>
</template>

<style>
.footer-top{
    
    background-image: url('/img/footer-bg.jpg');
    background-size: cover;
    .container{
        display: flex;
        justify-content: space-between;
    }
    #first-list{
        display: flex;
        flex-flow: column;
        justify-content: center;
        #title-list{
            color: white;
            margin-bottom: 20px;
        }
        li{
            color: #ffffff40;
            list-style-type: none;
        }
        .logo{
            z-index: 999;
            object-fit: cover;
            
        }
    }
    
}

</style>