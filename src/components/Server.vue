<template>
  <div class="grid grid-cols-3">
    <div class="col-span-3 lg:col-span-1 mb-5 lg:mb-0" v-for="server in servers" :key="server.name">

      <div class="mx-5 border-2 border-gray-200 shadow-md hover:shadow-2xl ease-in-out duration-300 rounded-lg">
        <div class="border-b-2">
          <h3 class="text-left text-2xl font-bold px-5 py-2">{{ server.name }}</h3>
        </div>
        <div class="px-5 py-4">
          <ul>
            <li>
              <span class="font-bold">游戏版本：</span>
              <span class="select-all">{{ server.version }}</span>
            </li>
            <li class="mt-2">
              <span class="font-bold">简单介绍：</span>
              <span>{{ server.intro }}</span>
            </li>
            <li class="mt-2">
              <span class="font-bold">连接地址：</span>
              <span class="select-all">{{ server.address }}</span>
            </li>
            <li class="mt-2">
              <span class="font-bold">注册：</span>
              <span class="select-all">{{ server.register }}</span>
            </li>
            <li class="mt-2">
              <span class="font-bold">登录：</span>
              <span class="select-all">{{ server.login }}</span>
            </li>
            <li class="mt-2" v-if="server.join && server.join !== ''">
              <span class="font-bold">进入子服：</span>
              <span class="select-all">{{ server.join }}</span>
            </li>
          </ul>
        </div>
      </div>

    </div>
  </div>
</template>

<script setup>

const servers = [
  {
    name: '群组服-生存子服',
    address: 'mc.cjlu.cc',
    intro: '纯净生存',
    version: '1.20.2',
    register: '/register 密码 重复密码',
    login: '/login 密码',
    join: '/join',
  }, {
    name: '群组服-创造子服',
    address: 'mc.cjlu.cc',
    intro: '复刻创造',
    version: '1.19.2',
    register: '/register 密码 重复密码',
    login: '/login 密码',
    join: '/join',
  }, {
    name: '暑期冒险',
    address: '59x-02.mcstory.cc:25303',
    intro: '暑期冒险整合包服',
    version: '1.19.2',
    register: '/register 密码 重复密码',
    login: '/login 密码',
    join: '/join',
  }
]

</script>

<style scoped>

</style>