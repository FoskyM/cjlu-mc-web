<template>

    <div class="mt-10">
      <a href="https://minecraftlist.com/servers/59x-02.mcstory.cc:13652" title="Minecraft server">
        <img src="https://minecraftlist.com/servers/59x-02.mcstory.cc:13652/banner@2x.jpg" alt="Minecraft server" class="w-full md:w-4/6 lg:w-3/6 mx-auto shadow-md hover:shadow-2xl ease-in-out duration-300"/>
      </a>
    </div>

  <div class="mt-10">
    <div class="border-2 border-gray-600 shadow-md rounded-2xl">
      <div class="border-b-2">
        <h3 class="text-left text-2xl font-bold px-5 py-2">关于我们</h3>
      </div>
      <div class=" px-5 py-2">
        E-sports达人社-MC部，由中国计量大学学生自发组建，并建立校MC服务器。
      </div>
    </div>
  </div>

  <div class="mt-10">
    <div class="border-2 border-gray-600 shadow-md rounded-2xl">
      <div class="border-b-2">
        <h3 class="text-left text-2xl font-bold px-5 py-2">服务器列表</h3>
      </div>
      <div class="px-5 py-5">

        <Server />

      </div>
    </div>
  </div>

</template>

<script setup>

import Server from "@/components/Server.vue";
</script>