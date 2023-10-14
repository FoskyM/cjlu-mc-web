<template>

    <div class="mt-10">
      <a href="https://www.mclists.cn/server/7086.html" target="_blank" title="Minecraft server">
        <img src="https://api.fosky.top/api/minecraft/image?address=mc.cjlu.cc" alt="Minecraft server" class="w-full md:w-4/6 lg:w-3/6 mx-auto shadow-md hover:shadow-2xl ease-in-out duration-300"/>
      </a>
    </div>

  <div class="mt-5">
    <a href="#" target="_blank" title="Minecraft server">
      <img src="https://api.fosky.top/api/minecraft/image?address=life.mc.cjlu.cc" alt="Minecraft server" class="w-full md:w-4/6 lg:w-3/6 mx-auto shadow-md hover:shadow-2xl ease-in-out duration-300"/>
    </a>
  </div>

  <div class="mt-10">
    <div class="border-2 border-gray-600 shadow-md rounded-xl">
      <div class="border-b-2">
        <h3 class="text-left text-2xl font-bold px-5 py-2">关于我们</h3>
      </div>
      <div class="px-5 py-2">
        E-sports 达人社所属MC部，由中国计量大学学生自发组建于 2022 年，并建立校MC服务器，首次开服于 2022.10.14。

      </div>
    </div>
  </div>

  <div class="mt-10">
    <div class="border-2 border-gray-600 shadow-md rounded-xl">
      <div class="border-b-2">
        <h3 class="text-left text-2xl font-bold px-5 py-2">服务器列表</h3>
      </div>
      <div class="py-5 px-2 md:px-5">

        <Server />

      </div>
    </div>
  </div>

  <div class="mt-10">
    <div class="border-2 border-gray-600 shadow-md rounded-xl">
      <div class="border-b-2">
        <h3 class="text-left text-2xl font-bold px-5 py-2">认证流程</h3>
      </div>
      <div class="px-5 py-2">
        <b class="py-1 text-lg">为何需认证？</b>
        <p>为了保证服务器的稳定性，我们需要对玩家进行认证，以防止恶意破坏。</p>
        <div class="py-2"></div>
        <b class="py-1 text-lg">如何认证？</b>
        <p>首先打开 <a class="underline underline-offset-2" href="https://bbs.cjlu.cc" target="_blank">量见论坛</a> 注册账号。</p>
        <p>其次在论坛进行认证，绑定学校 <a class="underline underline-offset-2" href="https://authserver.cjlu.edu.cn/" target="_blank" rel="noreferrer">统一认证</a> 账号，以验证你的身份。</p>
        <p>在游戏内注册登录后输入 <span class="select-all text-red-400 bg-red-100 py-0.5 px-1.5 rounded">/bind 论坛用户名 论坛密码</span> 即可。</p>
      </div>
    </div>
  </div>

</template>

<script setup>

import Server from "@/components/Server.vue";
</script>