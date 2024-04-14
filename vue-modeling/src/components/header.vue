<template>
     <header class="flex justify-between border-b border-slate-200 px-10 py-8">
    <div class="flex items-center gap-4">
      <img src="/public/logo.png"  alt="" class="w-10"/>
      <div>
        <h2 class="text-xl font-bold uppercasew">Vue-modeling</h2>
        <p class="text-slate-500">Магазин лучших 3D моделей</p>
      </div>
    </div>

    <ul class="flex items-center gap-10">
      <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img src="/public/cart.svg" alt="">
        <b>1205руб</b>
      </li>
      <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img src="/public/heart.svg" alt="">
        <span>Закладки</span>
      </li>
      <li class="flex items-center gap-3 cursor-pointer text-gray-500 hover:text-black">
        <img src="/public/heart.svg" alt="">
        <span>Профиль</span>
      </li>
    </ul>


  </header>
</template>