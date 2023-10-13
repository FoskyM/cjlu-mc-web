<template>
  <div class="mt-10">
    <div class="grid grid-cols-3">
      <div class="col-span-3 lg:col-span-1 mb-5" v-for="video in videos" :key="video.avid">
        <a :href="`https://www.bilibili.com/video/${video.bvid}`" target="_blank">
          <div class="mx-5 border-2 border-gray-200 shadow-md hover:shadow-2xl ease-in-out duration-300 rounded-lg">
            <img :src="video.pic" alt="" class="w-full"/>
            <div class="border-b-2">
              <h3 class="text-left text-sm font-bold px-5 py-2">{{ video.title }}</h3>
            </div>
            <div class="px-5 py-2 text-xs flex justify-between">
              <span>
                <a class="text-gray-800 hover:text-blue-500 ease-in-out duration-300" :href="`https://space.bilibili.com/${video.author_id}`" target="_blank">@{{ video.author }}</a>
              </span>
              <span>
                {{video.time}}
              </span>
            </div>
          </div>
        </a>
      </div>
    </div>
  </div>

</template>

<script setup>

const videos = [
  {
    avid: 859974444,
    bvid: 'BV1VG4y1f71i',
    title: '【中国计量大学服务器】史莱姆农场空置域的记录',
    pic: new URL(`@/assets/video-cover/afd0dc9fc379a8070bd0e7ea05eae8ddb1e17d33.jpg`, import.meta.url).href,
    time: '2022-11-08 21:26:45',
    author: '随便不是猪',
    author_id: 338956888
  },
  {
    avid: 776755575,
    bvid: 'BV1u14y1w76v',
    title: '[中国计量大学服务器]12.26双旦活动第一弹',
    pic: new URL(`@/assets/video-cover/9f1d01b7db1476e1e7ae18dbb30b0c27a4acacec.jpg`, import.meta.url).href,
    time: '2022-12-27 12:01:35',
    author: '19seconds',
    author_id: 502608050
  },
  {
    avid: 733126289,
    bvid: 'BV13D4y1v7pw',
    title: '计量大学MC服务器成果剪辑',
    pic: new URL(`@/assets/video-cover/3d2799c01502d1a2d9cd5b150de299d7b0f94551.jpg`, import.meta.url).href,
    time: '2022-12-27 12:01:35',
    author: '论史蒂夫的鞘翅力学',
    author_id: 1982757134
  },
  {
    avid: 774399607,
    bvid: 'BV1j14y157im',
    title: '【计量大学服务器】浏览玩家的建筑成果',
    pic: new URL(`@/assets/video-cover/b38a575148ae63f6b61540659d3acc12c6cb6902.jpg`, import.meta.url).href,
    time: '2022-10-25 12:12:25',
    author: '随便不是猪',
    author_id: 338956888
  },
  {
    avid: 608678763,
    bvid: 'BV1j84y1j7Zj',
    title: '大学服务器居然有这么多逆天建筑',
    pic: new URL(`@/assets/video-cover/2e8132a5700fc9dda6bed8d8353b302bf1706bee.jpg`, import.meta.url).href,
    time: '2023-02-02 14:56:53',
    author: '随便不是猪',
    author_id: 338956888
  }
]

</script>


<style scoped>

</style>