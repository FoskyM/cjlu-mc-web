<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="bg-gray-100 h-16 flex text-black-800 px-5 shadow-md px-0 md:px-40">
    <img alt="logo" src="@/assets/logo.jpg" class="h-full hidden" />
    <h1 class="text-2xl font-bold my-auto ml-2">CJLU MC</h1>
      <nav class="my-auto ml-5 flex items-center">
        <RouterLink to="/" class="bg-gray-200/75 hover:bg-gray-300 mx-1 px-5 py-2 rounded-lg">首页</RouterLink>
        <RouterLink to="/about" class="bg-gray-200/75 hover:bg-gray-300 mx-1 px-5 py-2 rounded-lg">关于</RouterLink>
        <RouterLink to="/history" class="bg-gray-200/75 hover:bg-gray-300 mx-1 px-5 py-2 rounded-lg">历程</RouterLink>
      </nav>

  </header>

  <RouterView />
</template>

<style scoped>

</style>
