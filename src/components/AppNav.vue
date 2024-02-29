<script>
    export default{
        nome:'AppNav',
    }
</script>

<template>
    <nav>
        <img src="/img/dc-logo.png" alt="Logo DC">
        <ul>
            <li>
                <a href="">ciao</a>
            </li>
            <li>
                <a href="">ciao</a>
            </li><li>
                <a href="">ciao</a>
            </li><li>
                <a href="">ciao</a>
            </li><li>
                <a href="">ciao</a>
            </li><li>
                <a href="">ciao</a>
            </li>
        </ul>
    </nav>
</template>

<style>
 nav{
    height: 100px;
    display: flex;
    img{
        height: 100%;;
    }
    ul{
        display: flex;
        gap: 10px;
        list-style-type: none;
        a{
            text-decoration: none;
    }
 }
}

 
</style>