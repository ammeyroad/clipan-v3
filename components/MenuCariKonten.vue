<template>
  <div>
    <input v-model="searchTerm" type="search" class="block w-full p-4 text-sm text-gray-900 border border-gray-300 rounded-lg bg-gray-50 focus:ring-blue-500 focus:border-blue-500" placeholder="sisa angsuran">
    <ul v-if="filteredList.length > 0" class="h-96 absolute overflow-y-auto mt-2 p-2 bg-white rounded-xl">
      <li v-for="item in filteredList" :key="item.judul" class="w-80 bg-white py-4 px-4 border-b border-1 border-gray-300 text-gray-500 hover:text-blue-700 shadow-none ">
        <router-link :to="item.to" class="flex justify-between  items-center group">
          <p class="font-semibold grid">
            {{ item.judul }} <span class="text-xs font-normal">{{ item.to }}</span>
          </p> <Icon name="line-md:upload-loop" class="w-8 h-8 group-hover:rotate-90 group-hover:opacity-100 opacity-0 duration-200" />
        </router-link>
      </li>
    </ul>
    <div v-else class="absolute text-gray-500 mt-2 p-2 bg-white rounded-xl" /><div class="w-80 bg-white py-4 px-4 border-1 border-gray-300 text-red-500 hover:text-blue-700 shadow-none ">
      <div class="flex justify-between  items-center group">
        <p class="font-semibold grid">
          Maaf, belum tersedia
        </p>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue'

const data = [
  {
    judul: 'Informasi saham',
    to: '/tata-kelola#tentang'
  },
  {
    judul: 'Laporan Tahunan',
    to: '/tata-kelola#visimisi'
  },
  {
    judul: 'Laporan keuangan',
    to: '/tata-kelola#vmanajemen'
  },
  {
    judul: 'Prospektus',
    to: '/tata-kelola#visimisi'
  },
  {
    judul: 'Laporan Tahunan',
    to: '/tata-kelola#visimisi'
  },
  {
    judul: 'Laporan keuangan',
    to: '/tata-kelola#vmanajemen'
  }
]

const searchTerm = ref('')

const filteredList = computed(() => {
  return data.filter(item => item.judul.toLowerCase().includes(searchTerm.value.toLowerCase()))
})
</script>
