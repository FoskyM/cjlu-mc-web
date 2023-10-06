<template>

  <div class="mt-5 px-28 min-h-[36rem] flex items-center">
    <ul class="list-disc">
      <li class="mt-2" v-for="log in logs.reverse()" :key="log">
        <span class="font-bold">{{ log.time }}：</span>
        <span>{{ log.content }}</span>
      </li>
    </ul>
  </div>

</template>

<script setup>
const logs = [
  {
    time: '2022',
    content: '服务器建立'
  },{
    time: '2023.10',
    content: '1.20.2 新周目纯净生存'
  }
]
</script>

<style scoped>

</style>