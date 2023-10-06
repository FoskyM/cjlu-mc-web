<template>
  <div class="mt-10">
    <div v-for="album in albums" :key="album">
      <h3 class="text-2xl">
        {{ album.name }}
        <span class="text-sm text-gray-500">by {{ album.author }}</span>
      </h3>

      <div class="mt-5"></div>

      <div class="grid grid-cols-3">
        <div class="col-span-3 lg:col-span-1 mb-5" v-for="photo in album.photos" :key="photo">
          <a :href="photo.src" target="_blank">
            <div class="mx-5 border-2 border-gray-200 shadow-md hover:shadow-2xl ease-in-out duration-300 rounded-lg">
              <img :src="photo.src" alt="" class="w-full"/>

              <div class="px-5 py-2 text-xs flex justify-end">

                <span>
                {{photo.alt}}
              </span>
              </div>
            </div>
          </a>
        </div>
      </div>
    </div>
  </div>

</template>

<script setup>

const photo_group = [
  '2022-10-14_22.01.20',
  '2022-10-14_22.01.54'
]

const photo_foskym = [
  '2022-10-14_23.32.10',
  '2022-10-14_23.33.32',
  '2022-10-14_23.41.37',
  '2022-10-16_21.58.09',
  '2022-10-18_17.09.24',
  '2022-10-18_17.10.04',
  '2022-10-18_17.11.46',
  '2022-10-18_21.11.10',
  '2022-10-21_18.02.05',
  '2022-10-21_19.08.49',
  '2022-10-24_22.11.17',
  '2022-10-29_13.45.00',
  '2023-05-12_18.01.33',
  '2023-05-14_13.11.42',
  '2023-08-16_21.34.49',
]

const albums = [
  {
    name: '合照',
    author: '全体成员',
    photos: photo_group.map((photo) => {
      return {
        src: new URL(`../assets/photo/group/${photo}.png`, import.meta.url).href,
        alt: photo
      }
    })
  }, {
    name: '一周目截图',
    author: 'FoskyM',
    photos: photo_foskym.map((photo) => {
      return {
        src: new URL(`../assets/photo/FoskyM/${photo}.png`, import.meta.url).href,
        alt: photo
      }
    })
  }
]

</script>

<style scoped>

</style>