<script>
import AppNav from './components/AppNav.vue'

//importo l'header
import AppHeader from './components/AppHeader.vue';

// importo il m ain delle schede
import AppMain from './components/AppMain.vue';
 
//importo il footerTop
import AddFooterTop from './components/AddFooterTop.vue';

//importo il footerBottom
import AddFooterBottom from './components/AddFooterBottom.vue';



export default{
    components: {
                AppNav,
                AppHeader,
                AppMain,
                AddFooterTop,
                AddFooterBottom,
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
        <AddFooterTop></AddFooterTop>
        <AddFooterBottom></AddFooterBottom>
</template>

<style lang="scss">

@use './styles/general.scss';

</style>