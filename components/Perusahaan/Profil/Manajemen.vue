<template>
  <section class="py-24">
    <div class="max-w-screen-lg mx-auto pl-4">
      <div class="sm:text-center text-left mb-10">
        <span
          class="
            bg-yellow-400
            text-black text-xs
            font-medium
            mr-2
            px-2.5
            py-1.5
            rounded-full
          "
          >Manajemen Clipan</span
        >

        <h1 class="hed3 mt-4">jajaran direksi dan komisaris</h1>
        <garis />

        <h3 class="pr-8 sm:px-32 pb-5 hed4">
          Kinerja Clipan tidak lepas dari peranan jajaran Komisaris dan Direksi
          yang Dewan Komisaris dan Direksi berpengalaman, berprestasi, dan pakar
          di bidangnya.
        </h3>
      </div>
      <div class="sm:text-center text-left mb-10">
        <span
          class="
            bg-yellow-400
            text-black text-xs
            font-medium
            mr-2
            px-2.5
            py-1.5
            rounded-full
          "
          >Investor dan Korporasi</span
        >

        <h1 class="hed3 mt-4">Informasi RUPS dan Berita lainnya</h1>
        <garis />

        <h3 class="pr-8 sm:px-32 pb-5 hed4">
          Informasi bagi investor, masyarakat pasar modal dan pemegang saham
          disajikan dengan transparan
        </h3>
      </div>
      <TabGroup>
        <TabList class="flex space-x-1 rounded-xl p-1 mr-4 sm:mr-0">
          <Tab
            :class="[
              'w-full rounded-lg py-2.5 text-sm font-medium leading-5 text-blue-700',
              'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
              selected
                ? 'bg-white shadow'
                : 'text-blue-100 hover:bg-white/[0.12] hover:text-white',
            ]"
            >Tab 1</Tab
          >
          <Tab
            :class="[
              'w-full rounded-lg py-2.5 text-sm font-medium leading-5 text-blue-700',
              'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
              selected
                ? 'bg-white shadow'
                : 'text-blue-100 hover:bg-white/[0.12] hover:text-white',
            ]"
            >Tab 2</Tab
          >
          <Tab
            :class="[
              'w-full rounded-lg py-2.5 text-sm font-medium leading-5 text-blue-700',
              'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
              selected
                ? 'bg-white shadow'
                : 'text-blue-100 hover:bg-white/[0.12] hover:text-white',
            ]"
            >Tab 3</Tab
          >
        </TabList>
        <TabPanels>
          <TabPanel> <PerusahaanProfilManajemenKoms /></TabPanel>
          <TabPanel><PerusahaanProfilManajemenDir />asas</TabPanel>
          <TabPanel><PerusahaanProfilManajemenEvp /></TabPanel>
        </TabPanels>
      </TabGroup>
    </div>
  </section>
</template>

<script setup>
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue';
const komisaris = [
  {
    nama: 'Roosniati Salihin',
    jabatan: 'Komisaris utama',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/woman1.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
  {
    nama: 'Mukmin Ali Gunawan',
    jabatan: 'Komisaris',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/man.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
  {
    nama: 'Mukmin Ali Gunawan',
    jabatan: 'Komisaris',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/woman.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
  {
    nama: 'Mukmin Ali Gunawan',
    jabatan: 'Komisaris',
    foto: 'https://tailus.io/sources/blocks/leadership/preview/images/woman1.jpg',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik perusahaan sesuai dengan prinsip-prinsip.',
  },
];
</script>
