<template>
    <div>
        <h1>{{post.citation}}</h1>
        <h2> {{post.authors}}</h2>
    
    </div>
</template>

<script>
export default {
    name : 'Index',
    props : ['post']
}
</script>

<style>

</style>
