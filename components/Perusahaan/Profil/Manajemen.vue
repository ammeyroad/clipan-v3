<template>
  <section class="py-24">
    <div class="max-w-screen-lg mx-auto pl-4">
      <div class="sm:text-center text-left mb-10">
        <div
          class="
            inline-flex
            justify-between
            items-center
            py-1
            px-1
            text-sm text-gray-700
            bg-white
            rounded-full
          "
          role="alert"
        >
          <span
            class="
              text-xs
              bg-yellow-400
              rounded-full
              text-black
              font-semibold
              px-4
              py-1.5
              mr-3
            "
            >Manajemen</span
          >
          <span class="text-sm font-medium mr-2">level Atas</span>
        </div>

        <h3 class="">jajaran direksi dan komisaris</h3>
        <garis />

        <p class="pr-8 sm:px-32 pb-5">
          Berawal dari marketplace lalu tumbuh menjadi platform yang memberikan
          banyak kemudahan untuk berbisnis. Inilah kami,
        </p>
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
          <TabPanel>
            <div
              class="
                flex
                py-12
                w-full
                md:mx-auto md:max-w-screen-xl
                overflow-x-auto
              "
            >
              <div class="flex space-x-4">
                <div
                  v-for="item in komisaris"
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
                      group-hover:-translate-y-0 group-hover:bg-blue-600/80
                    "
                  >
                    <div class="">
                      <h4
                        class="
                          text-lg
                          font-semibold
                          dark:text-gray-700
                          text-white
                        "
                      >
                        {{ item.nama }}
                      </h4>
                      <span class="block text-sm text-white">{{
                        item.jabatan
                      }}</span>
                    </div>
                    <p class="mt-4 text-sm text-white">
                      {{ item.isi }}
                    </p>
                  </div>
                </div>
              </div>
            </div></TabPanel
          >
          <TabPanel>Content 2</TabPanel>
          <TabPanel>Content 3</TabPanel>
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
