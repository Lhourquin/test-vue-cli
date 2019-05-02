<template>
    <div class="nav">
        <nav><a href="">Accueil</a>
        <a href="">Contact</a>
        <a href="">A propos</a>
        <a href="">Portfolio</a></nav>
    
    </div>
</template>

<script>
export default {
    name : 'NavBar',
}
</script>

<style>
.nav {
background-color : red;
grid-area: nav;
height : 100vh;
}
nav{
display : flex;
flex-direction: column;
}
</style>
