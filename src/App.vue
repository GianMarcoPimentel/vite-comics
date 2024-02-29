<script>
import AppNav from './components/AppNav.vue'

//importo l'header
import AppHeader from './components/AppHeader.vue';

// importo il m ain delle schede
import AppMain from './components/AppMain.vue';

//importo il footer


export default{
    components: {
                AppNav,
                AppHeader,
                AppMain,
                
            },
    data(){
        return{
            

        }
    }
}
</script>

<template>
    

        <AppNav></AppNav>
        <AppHeader></AppHeader>
        <AppMain></AppMain>
</template>

<style lang="scss">

@use './styles/general.scss';

</style>