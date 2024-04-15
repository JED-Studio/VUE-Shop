<template>
<Drawer />
<div class="lok bg-white w-4/5 m-auto rounded-xl shadow-xl mt-14">
  <Header />


  <div class="p-10">
<h2 class="text-3xl font-bold mb-8">Все модели</h2>
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

