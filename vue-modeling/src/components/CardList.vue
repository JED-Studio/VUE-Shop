<script setup>
import Card from './Card.vue';
</script>



<template>
    <div class="grid grid-cols-4 gap-5">
  <Card title="Мужские кроссвки Nike Blazer Mid Suede" 
  imageUrl="/public/sneakers/sneakers-1.jpg" 
  :price="1000" 
  :isFavorite="false" 
  :onClikAdd="onClikAdd" 
  :isAdded="true"/>
  <Card />
  <Card />
  <Card />
  <Card />
  <Card />
  <Card />
  <Card />
  <Card />
</div>
</template>