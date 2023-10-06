<template>
  <header class="bg-gray-100 h-10 md:h-16 flex text-black-800 px-5 shadow-md px-0 md:px-40">
    <img alt="logo" src="@/assets/logo.jpg" class="h-full mr-2 hidden"/>
    <h1 class="text-base md:text-2xl font-bold my-auto">CJLU MC</h1>
    <nav class="my-auto ml-2 md:ml-5 flex items-center">
      <RouterLink :to="link.url" class="bg-gray-200/75 hover:bg-gray-400/75 mx-0 md:mx-1 px-2 md:px-5 h-full py-2 rounded-none md:rounded-lg ease-in-out duration-300" :class="router.currentRoute.value.path === link.url ? 'bg-gray-300' : ''" v-for="link in route_links" :key="link.name">
        {{ link.name }}</RouterLink>
    </nav>

  </header>

  <div class="container">
    <RouterView/>
  </div>

  <Footer/>

</template>

<script setup>
import {RouterLink, RouterView} from 'vue-router'
import Footer from "@/components/Footer.vue";
import router from "@/router";

const route_links = [
  {
    name: "首页",
    url: "/"
  },
  {
    name: "实况",
    url: "/facts"
  },
  {
    name: "相册",
    url: "/photo"
  },
  {
    name: "历程",
    url: "/history"
  }
]
</script>

<style scoped>

</style>
