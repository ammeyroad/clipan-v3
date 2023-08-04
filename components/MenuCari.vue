<template>
  <div>
    <button type="button" class="bg-gray-100 hover:bg-blue-600 font-medium rounded-xl text-sm p-1.5 text-center inline-flex items-center text-blue-600 hover:text-white" @click="openModal">
      <Icon name="icon-park-twotone:search" class="w-8 h-8 p-1 " />
    </button>
    <div v-if="isModalOpen" class="fixed modal-overlay inset-0 flex items-center justify-center z-50">
      <div class="bg-gray-100 w-full h-full rounded-lg shadow-md p-6">
        <div class="flex items-center justify-between">
          <h4 class="font-black ">
            Kamu Cari Apa?
          </h4>
          <button class="bg-gray-300 hover:bg-gray-400 text-gray-800 font-medium py-2 px-4 rounded" @click="closeModal">
            x
          </button>
        </div>
        <p class="my-4">
          <MenuCariKonten />
        </p>
        <div class="flex justify-end" />
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const isModalOpen = ref(false)

const openModal = () => {
  isModalOpen.value = true
}

const closeModal = () => {
  isModalOpen.value = false
}
</script>

  <style>
    .modal-overlay {
      background-color: rgba(0, 0, 0, 0.954);
    }
  </style>
