<template>
  
  <h1>Archakov blog</h1>
  <Myhello title="Mersedez" :price="3000" :isAdded="true">
    <button>Добавить</button>
  </Myhello>
  <Myhello />
  <Myhello />
  <Myhello />
  <Myhello />
</template>

<script setup>

import Myhello from './components/Myhello.vue'

</script>

<style>
</style>