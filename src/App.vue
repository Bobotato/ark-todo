<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="grid grid-rows-[300px_1fr_1fr] bg-[#181818] justify-center p-5">
    <img src="src/assets/images/ArkChores.png" class="w-[500px] h-[300px] justify-self-center">
    <h1 class="text-center text-emerald-500 text-xl mt-5"> Welcome to the future of unpaid slave labour.</h1>
    <nav class="grid grid-cols-2 text-center mt-10">
      <RouterLink to="/" class="text-white cursor-pointer hover:text-emerald-300">TO DO LIST</RouterLink>
      <RouterLink to="/completed" class="text-white cursor-pointer hover:text-emerald-300">COMPLETED</RouterLink>
    </nav>
  </header>
  <RouterView/>
</template>

<style scoped>
</style>
