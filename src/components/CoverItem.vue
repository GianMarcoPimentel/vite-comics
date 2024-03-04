<script>
    export default{
        name:'CoverItem',
        // questo componente esige delle proprietà
        // in modo da essere visualizzato correttamente
        props: {
            coverImage: String,
            coverSerie: String,
        }
    }
</script>

<template>
             <div class="cover">
            
                <img :src="coverImage" alt="">
                <h4>{{coverSerie}}</h4>
            </div>
</template>

<style>
</style>