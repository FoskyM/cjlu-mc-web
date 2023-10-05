<template>
  <header class="bg-gray-100 h-16 flex text-black-800 px-5 shadow-md px-0 md:px-40">
    <img alt="logo" src="@/assets/logo.jpg" class="h-full mr-2 hidden"/>
    <h1 class="text-2xl font-bold my-auto">CJLU MC</h1>
    <nav class="my-auto ml-5 flex items-center">
      <RouterLink :to="link.url" class="bg-gray-200/75 hover:bg-gray-300 mx-1 px-5 py-2 rounded-lg ease-in-out duration-300" v-for="link in route_links" :key="link.name">
        {{ link.name }}</RouterLink>
    </nav>

  </header>

  <div class="container ">
    <RouterView/>
  </div>

  <Footer/>

</template>

<script setup>
import {RouterLink, RouterView} from 'vue-router'
import Footer from "@/components/Footer.vue";

const route_links = [
  {
    name: "首页",
    url: "/"
  },
  {
    name: "关于",
    url: "/about"
  },
  {
    name: "历程",
    url: "/history"
  }
]
</script>

<style scoped>

</style>
