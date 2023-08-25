<template>
  <div class="flex py-12 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
    <div class="flex space-x-4">
      <div
        v-for="item in direksi"
        class="
          group
          relative
          rounded-xl
          hover:shadow-2xl
          w-72
          sm:w-full
          space-y-6
          overflow-hidden
        "
      >
        <img
          class="
            mx-auto
            h-[360px]
            sm:h-[330px]
            w-full
            grayscale-0
            object-cover object-top
            transition
            duration-500
            group-hover:scale-110 group-hover:grayscale
          "
          :src="item.foto"
          alt="woman"
          loading="lazy"
        />
        <div
          class="
            absolute
            bottom-0
            h-full
            mt-auto
            px-4
            py-2
            bg-blue-600
            translate-y-72
            sm:translate-y-64
            transition
            duration-300
            ease-in-out
            duration-200
            group-hover:-translate-y-0 group-hover:bg-blue-600/80
          "
        >
          <div class="">
            <h4 class="text-lg font-semibold dark:text-gray-700 text-white">
              {{ item.nama }}sdasdsa
            </h4>
            <span class="block text-sm text-white">{{ item.jabatan }}</span>
          </div>
          <p class="mt-4 text-sm text-white">
            {{ item.isi }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue';
const direksi = [
  {
    nama: 'Harjanto Tjitohardjojo',
    jabatan: 'Direktur utama',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/man.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
  {
    nama: 'Jahja Anwar',
    jabatan: 'Direksi',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/woman1.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
  {
    nama: 'Engelbert Rorong Jr',
    jabatan: 'Direksi',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/woman.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
  {
    nama: 'Yimmy Weddianto',
    jabatan: 'Direksi',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/woman1.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
];
</script>
