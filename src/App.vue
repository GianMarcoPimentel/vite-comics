<script>
import AppNav from './components/AppNav.vue';

//importo l'header
import AppHeader from './components/AppHeader.vue';
export default{
    components: {
                AppNav,
                AppHeader,
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
   
</template>

<style lang="scss">

@use './styles/general.scss';

</style>