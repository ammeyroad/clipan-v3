<template>
  <section class="">
    <div
      class="
        bg-blue-600
        h-52
        sm:h-[400px]
        bg-[url('/background-slider.jpg')] bg-cover bg-no-repeat bg-center
      "
    >
      <div class="flex items-center mx-auto max-w-screen-xl">
        <div class="sm:w-1/2 pt-24 px-6 sm:pt-24">
          <div class="flex text-white">
            <a href="#" title="Back to homepage" class="hover:underline">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 20 20"
                fill="currentColor"
                class="w-5 h-5 pr-1 dark:text-gray-400"
              >
                <path
                  d="M10.707 2.293a1 1 0 00-1.414 0l-7 7a1 1 0 001.414 1.414L4 10.414V17a1 1 0 001 1h2a1 1 0 001-1v-2a1 1 0 011-1h2a1 1 0 011 1v2a1 1 0 001 1h2a1 1 0 001-1v-6.586l.293.293a1 1 0 001.414-1.414l-7-7z"
                />
              </svg>
            </a>
            /
            <a
              rel="noopener noreferrer"
              href="#"
              class="flex items-center px-1 capitalize hover:underline ml-2"
              >Profile</a
            >
            /
          </div>
          <h3 class="text-black text-yellow-400">Profile Perusahaan</h3>
        </div>
        <div class="sm:w-1/2">
          <img
            src="/slider-1.png"
            loading="lazy"
            class="hidden sm:flex h-[400px] mx-auto"
          />
        </div>
      </div>
    </div>
  </section>
  <section
    class="
      flex
      w-full
      sticky
      top-14
      sm:top-20
      bg-blue-50
      z-10
      md:mx-auto md:max-w-screen-xl
      overflow-x-auto
    "
  >
    <div class="flex pt-4 pb-1 sm:pb-4 pl-4 sm:mx-auto">
      <nuxt-link
        to="#section1"
        v-for="sub in submenus"
        class="
          bg-transparent
          ring-1 ring-blue-600
          py-2
          rounded-2xl
          px-4
          mr-3
          mb-0
          text-sm
          hover:bg-blue-600 hover:text-white
          duration-300
          text-center
          mx-auto
        "
      >
        <p class="w-max">{{ sub.nama }}</p>
      </nuxt-link>
    </div>
  </section>
</template>
<script setup>
const submenus = [
  {
    nama: 'Sejarah Clipan',
    link: '#sejarah',
  },
  {
    nama: 'Visi Misi & Budaya',
    link: '#visi',
  },
  {
    nama: 'Profil Manajemen',
    link: '#profil',
  },
  {
    nama: 'Penghargaan',
    link: '#penghargaan',
  },
];
</script>
