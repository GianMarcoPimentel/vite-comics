<script>
    export default {
        nome: 'AppFooter',
        data(){
        return {
            symbols:[
                "/img/footer-facebook.png",
                "/img/footer-twitter.png",
                "/img/footer-youtube.png",
                "/img/footer-pinterest.png",
                "/img/footer-periscope.png",
        ]
        
        
        }
    }
    }
</script>

<template>
<footer>
    <div class="container">
        <div class="footer-bottom">
            <button class="btn"> Sign-up now!</button>
            <div class="siti">
                <span>FOLLOW US</span>
                
                <div v-for="symbol in symbols"> 
                    <img :src="symbol" alt="">
                </div>
                
            </div>
        </div>
    </div>
</footer>
</template>

<style>
footer{
    
    background-color: #303030;
    .footer-bottom{
        display: flex;
        justify-content: space-between;
        align-items: center;

        padding: 30px 0px;
    }
    .btn{
        padding: 20px;
        border: 3px #0282F9 solid;
        background-color: #303030;

        color: white;
        text-transform: uppercase;
    }
    .siti{
        display: flex;
        align-items: center;
        gap: 10px;
        color: #0282F9;
    }
}

</style>