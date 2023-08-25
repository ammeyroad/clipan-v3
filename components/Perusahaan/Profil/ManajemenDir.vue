<template>
  <div class="flex py-12 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
     <div class="flex space-x-4 sm:justify-center">
      <div
        v-for="item in direksi"
        class="
          group
          relative
          rounded-xl
          hover:shadow-xl
          w-72
          sm:w-1/4
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
        />
        <div
          class="
            absolute
            bottom-0
            h-full
            mt-auto
            px-4
            py-2
            bg-amber-400
            translate-y-72
            sm:translate-y-64
            transition
            duration-300
            ease-in-out
            group-hover:-translate-y-0 group-hover:bg-amber-400/80
          "
        >
          <div class="text-center">
            <h4 class="text-lg font-bold text-black">
              {{ item.nama }}
            </h4>
            <span class="block text-sm text-blue-600">{{ item.jabatan }}</span>
          </div>

          <p class="pt-3 mt-2 text-black text-xs w-full">
            <b>Riwayat:</b> <br />
        <p v-html="item.riwayat"></p>
          </p>
          <p class="pt-3 text-xs text-black">
            <b>Pendidikan:</b> <br />
           <p v-html="item.pendidikan"></p>
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
    jabatan: 'Direktur Utama',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Operation Director Tunas Toyota (2004-2006) <br> • Vice President di Tunas Toyota (2006-2010) <br> • Marketing and Sales Director di PT Mandiri Tunas Finance (2010-2021).',
    pendidikan: 'Sarjana Ekonomi dari Fakultas Ekonomi, Jurusan Manajemen, Universitas Krida Wacana Jakarta (1991)',
  },
  {
    nama: 'Jahja Anwar',
    jabatan: 'Direktur',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Country Manager di Wells Fargo Bank (2004-2012) <br> • Executive Vice President di Perseroan (2012-2013) <br> • Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
    pendidikan: 'Master of Business Adminstration (MBA) dari De Paul University Of Chicago, Amerika Serikat (1990).'
  },
    {
    nama: 'Engelbert Rorong, Jr',
    jabatan: 'Direktur',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: '• Senior Manager di Perseroan (2006-2009)<br> • Executive Vice President di Perseroan (2009-2013)<br> • Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
    pendidikan: 'Beliau merupakan lulusan dari STIE PERBANAS, Jakarta (1992)',
  },
  {
    nama: 'Yimmy Weddianto',
    jabatan: 'Direktur',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Area Manager di PT Nissan Motor Distributor Indonesia (2002-2005) <br> • Senior Vice President di PT Adira Dinamika Multifinance Tbk (2005-2016) <br> • Diangkat sebagai Direktur Perseroan sejak 2016.',
    pendidikan: 'Sarjana Teknik, Jurusan Teknik Industri dari Fakultas Teknik UniversitasTrisakti, Jakarta (2000).'
  },
];
</script>
