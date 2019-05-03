<template>
    <div class="button1">
        <h1>okok</h1>
        <button  
  v-on:click="$emit('test')"
  >test</button>
    </div>
</template>

<script>
export default {
    name : 'Button',
    
}
</script>

<style>
.button1{
grid-area : button1;
}
</style>
