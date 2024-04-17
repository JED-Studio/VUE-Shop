<template>
<!--<Drawer />-->
<div class="lok bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
  <Header />


  <div class="p-10">
    <div class="flex justify-between">
      <h2 class="text-3xl font-bold mb-8">Все модели</h2>
<div>
      <select class="py-2 px-3 border rounded-md outline-none">
        <option>По названию</option>
        <option>По цене (дешевые)</option>
        <option>По цене (дорогие)</option>
      </select>

      <div class="relative">
        <img class="absolute left-4 top-3" src="/public/search.svg" alt="" />
        <input class="border rounded-md py-2 pl-11 pr-4 outline-none focus:border-gray-400" type="text" placeholder="Поиск..."/>
      </div>
    
    </div>
</div>
    <CardList />
  </div>
</div>

</template>

<script setup>

import Drawer from './components/Drawer.vue';
import CardList from './components/CardList.vue'
import Header from './components/Header.vue';
import Myhello from './components/Myhello.vue'

</script>

