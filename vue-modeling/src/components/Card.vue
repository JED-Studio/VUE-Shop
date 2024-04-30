
<script setup>

import { inject } from 'vue';

const props = defineProps({
  id: Number,
  title: String,
  imageUrl: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClikAdd: Function,
  onClikFavorite: Function,


 
})


const addToFavorite = inject('addToFavorite')

const onClikFavorite =  () => {
  const obj = {
    ...props,
    parentId: props.id,
  }

  addToFavorite(obj);
}

</script>




<template>
    <div class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl">
      <img @click="onClikFavorite" :src="!isFavorite ? '/like-1.svg' : '/like-2.svg'" alt="Plus" class="absolute top-3 left-8" />

    
    <img :src="imageUrl" alt="Sneaker">
    <p class="mt-2">{{ title }}</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Цена:</span>
        <b>{{ price }}</b>
      </div>

      <img @click="onClikAdd" :src="!isAdded ? '/plus.svg' : '/checked.svg'" alt="Plus" />
    </div>
  </div>
</template>