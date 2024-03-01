<script>
export default{
        nome:'AppHeader',
        
    }
</script>

<template>
    <header>
        <div class="container">
            <span id="content"> Content goes her </span>
        </div>
    </header>
</template>

<style scope>
    #content{ 
        height: 100%;
        display: flex;
        align-items: center;
        font-size: 1.3em;
        
        &::before{
            content: '--> ';
            margin-right: 10px
        };
        &::after{
            content: ' <--';
            margin-left: 10px;
        }
    }
</style>