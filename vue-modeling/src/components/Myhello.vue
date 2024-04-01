<!--
<script>
export default{
    data(){
        return{
            count: 0
        }
    },
    methods:{
        increment(){
            this.count++;
        }
    }
}
</script>
-->
<script setup>

import {ref} from 'vue'

const count = ref(0)

function increment(){
    count.value++
}

</script>



<template>

<h1>{{ count }}</h1>
<button @click="increment">+</button>



</template>

<style scoped> /*scoped */

</style>


 