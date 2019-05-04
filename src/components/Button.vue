<template>
    <div  class="button1">
        <div 
     v-for="arr in arrk" 
     v-bind:key="arr.id">
       <h1>{{arr.id}}</h1> 
        </div>
        <button  
  v-on:click="$emit('test')"
  >test</button>
  <button
  v-on:click="displayRandom(arrs)">random</button>
  <button
  v-on:click="testEvent">push</button>
 
    </div>
    
</template>

<script>
export default {
    name : 'Button',
    data () {
        return {
            
            arrs : [ 
                1,
                2,
                3,
                4,
                5
            ],
             index : null,
             arrk : []
        }
       
    },
    methods : {
    displayRandom : function (items) {
    
        this.index = items [Math.floor(Math.random() * items.length)]
        console.log('index' + '=' + this.index)
        
        },
        pushRandom : function () {
            this.arrk.push({
                id : this.index
        })
        console.log(this.arrk)
        },
        popRandom : function () {
            if(this.arrk.length > 1)
            this.arrk.shift()
        },
        testEvent : function () {
            this.displayRandom(this.arrs)
            this.pushRandom()
            this.popRandom()
        }
}
}
    

</script>

<style>
.button1{
grid-area : button1;
}
</style>
