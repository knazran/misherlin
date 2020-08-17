<template>
  <div>
    <div class="mx-auto w-1/3 border-black border-4 px-4 py-2">
      <h1 class="text-center text-3xl tracking-widest font-bold">Full-time Foodie</h1>
    </div>
    <div id="nav" class="flex space-x-6 text-sm">
      <nuxt-link class="text-gray-700 hover:text-black" :to="`/`">HOME</nuxt-link>
      <a class="text-gray-700 hover:text-black">BLOG</a>
      <a class="text-gray-700 hover:text-black">ABOUT</a>
    </div>
    <div id="nav-hero" class="my-4">
      <img src="https://picsum.photos/1080/400" />
    </div>
  </div>
</template>