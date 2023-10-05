<template>
  <footer class="bg-gray-200 py-10 px-5 md:px-40 absolute bottom-0 w-full">
    <div class="grid grid-cols-3">
      <div class="col-span-3 md:col-span-1">
        <h3 class="text-xl py-2 font-bold">版权所有</h3>
        <p class="text-sm">&copy;Copyright 2022-2023 CJLU MC Server.</p>
      </div>

      <div class="col-span-3 md:col-span-1">
        <h3 class="text-xl py-2 font-bold">友情链接</h3>
        <ul class="text-sm">
          <li v-for="link in links" :key="link.name" class="mt-1.5">
            <a :href="link.url" target="_blank">{{ link.name }}</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script setup>
const links = [
  {
    name: "FoskyM",
    url: "https://fosky.top"
  },{
    name: "量见论坛",
    url: "https://bbs.cjlu.cc"
  }
]
</script>

<style scoped>

</style>