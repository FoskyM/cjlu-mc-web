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
    time: '2022.10.14',
    content: '服务器首次开放'
  }, {
    time: '2022.12.26',
    content: '双旦活动'
  }, {
    time: '2023.01.17',
    content: '宝可梦服务器开放'
  }, {
    time: '2023.03.18',
    content: 'ATM7 to the sky 整合包服务器开放'
  }, {
    time: '2023.05.20',
    content: '中国计量大学X水利水电院校MC联合委员会2023五二零活动特别企划之猎枪与獠牙'
  }, {
    time: '2023.07.27',
    content: 'Life in the village 3 整合包服务器开放'
  }, {
    time: '2023.10.03',
    content: '1.20.2 新周目纯净生存'
  }, {
    time: '2023.10.14',
    content: '一周年'
  }
]
</script>

<style scoped>

</style>