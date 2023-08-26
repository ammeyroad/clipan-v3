<template>
  <div class="w-full mx-auto max-w-screen-lg px-2 py-16 sm:px-0">
    <TabGroup>
      <TabList class="flex sm:justify-center space-x-1 rounded-xl p-1">
        <Tab
          v-for="category in Object.keys(categories)"
          as="template"
          :key="category"
          v-slot="{ selected }"
        >
          <button
            :class="[
              'w-full sm:w-max p-4  rounded-lg py-2.5 text-sm font-medium leading-5 text-blue-700',
              'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
              selected
                ? 'bg-white shadow'
                : 'text-blue-100 hover:bg-white/[0.12] hover:text-white',
            ]"
          >
            {{ category }}
          </button>
        </Tab>
      </TabList>

      <TabPanels class="mt-2">
        <TabPanel
          v-for="(posts, idx) in Object.values(categories)"
          :key="idx"
          :class="[
            'rounded-xl p-3',
            'ring-white ring-opacity-60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
          ]"
        >
          <div
            class="flex w-full md:mx-auto md:max-w-screen-xl overflow-x-auto"
          >
            <div class="flex space-x-4 sm:space-x-6 sm:justify-center">
              <div
                v-for="post in posts"
                :key="post.id"
                class="
                  group
                  relative
                  rounded-xl
                  hover:shadow-xl
                  w-64
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
                  :src="post.foto"
                />
                <div :class="[post.warna, 'absolute ease-in-out']">
                  <div class="text-center">
                    <div class="rounded-lg">
                      <h5 class="text-xl font-bold">
                        {{ post.nama }}
                      </h5>
                      <span class="block text-sm">{{ post.jabatan }}</span>
                    </div>
                    <div class="text-left pt-3 w-full p-2">
                      <p class="text-sm font-bold">Riwayat</p>
                      <p class="text-xs mb-2" v-html="post.riwayat"></p>
                      <p class="text-sm font-bold">Pendidikan</p>
                      <p class="text-xs mb-2" v-html="post.pendidikan"></p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </TabPanel>
      </TabPanels>
    </TabGroup>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue';

const categories = ref({
  KOMISARIS: [
    {
      id: 1,
      warna: 'tabkomisaris',
      nama: 'Roosniati Salihin',
      jabatan: 'Komisaris utama',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        'Memulai kariernya pada Divisi Internasional dan sebagai Executive Vice President di PT Bank Pan Indonesia Tbk (1991) sebelumnya Presiden Komisaris di PT Westpac Panin Bank (1991-1993)',
      pendidikan:
        '• Lulusan Bahasa Jepang dari Kokkusai Gakkuyukai, Tokyo, Jepang (1965) <br> • Lulusan English Literature dari University of California, Los Angeles, Amerika Serikat (1968)',
    },
    {
      warna: 'tabkomisaris',
      id: 2,
      nama: 'Bhindawati Gunawan',
      jabatan: 'Komisaris',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        '• Wakil Komisaris Utama PT Panin Financial Tbk (d/h PT Panin Life Tbk)(1991-2001) <br>• Menjabat sebagai Komisaris Utama Perusahaan (1991-2020) <br> dan • Menjabat sebagai Komisaris Perseroan (2020-sekarang)',
      pendidikan: 'Beliau merupakan lulusan Akademi Bisnis.',
    },
    {
      warna: 'tabkomisaris',
      id: 3,
      nama: 'Lukman Abdullah',
      jabatan: 'Komisaris Independen',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        '• Auditor di KAP Capelle Tuanakotta & Co. (1980-1990) <br> • Partner di KAP Drs. Hans Tuanakotta & Mustofa (1991-2002) <br> • Anggota Komite Audit di PT Asuransi Ramayana Tbk (2004-2008).',
      pendidikan:
        '• Sarjana Ekonomi dari Fakultas Ekonomi, Universitas Indonesia, Jakarta (1981)',
    },
  ],
  DIREKSI: [
    {
      warna: 'tabdireksi',
      id: 1,
      nama: 'Harjanto Tjitohardjojo',
      jabatan: 'Direktur Utama',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        'Operation Director Tunas Toyota (2004-2006) <br> • Vice President di Tunas Toyota (2006-2010) <br> • Marketing and Sales Director di PT Mandiri Tunas Finance (2010-2021).',
      pendidikan:
        'Sarjana Ekonomi dari Fakultas Ekonomi, Jurusan Manajemen, Universitas Krida Wacana Jakarta (1991)',
    },
    {
      warna: 'tabdireksi',
      id: 2,
      nama: 'Jahja Anwar',
      jabatan: 'Direktur',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        'Country Manager di Wells Fargo Bank (2004-2012) <br> • Executive Vice President di Perseroan (2012-2013) <br> • Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
      pendidikan:
        'Master of Business Adminstration (MBA) dari De Paul University Of Chicago, Amerika Serikat (1990).',
    },
    {
      warna: 'tabdireksi',
      id: 3,
      nama: 'Engelbert Rorong, Jr',
      jabatan: 'Direktur',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        '• Senior Manager di Perseroan (2006-2009)<br> • Executive Vice President di Perseroan (2009-2013)<br> • Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
      pendidikan: 'Beliau merupakan lulusan dari STIE PERBANAS, Jakarta (1992)',
    },
    {
      warna: 'tabdireksi',
      id: 4,
      nama: 'Yimmy Weddianto',
      jabatan: 'Direktur',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        'Area Manager di PT Nissan Motor Distributor Indonesia (2002-2005) <br> • Senior Vice President di PT Adira Dinamika Multifinance Tbk (2005-2016) <br> • Diangkat sebagai Direktur Perseroan sejak 2016.',
      pendidikan:
        'Sarjana Teknik, Jurusan Teknik Industri dari Fakultas Teknik UniversitasTrisakti, Jakarta (2000).',
    },
  ],
  EXECUTIVE: [
    {
       warna: 'tabevp',
      id: 1,
      nama: 'Donny Tri Wardono',
      jabatan: 'Executive Vice President',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        'Berbekal pengalaman lebih dari 27 tahun di bidang Sumber Daya Manusia (SDM), Beliau juga pernah menjabat posisi General Manager dan Senior General Manager di sejumlah perusahaan pembiayaan.',
      pendidikan:
        'Beliau meraih gelar Sarjana (S1) dari Universitas Diponegoro, Semarang pada tahun 1985 dan gelar Magister (S2) dari Universitas Gadjah Mada, Jakarta pada tahun 2003.',
    },
    {
       warna: 'tabevp',
      id: 2,
      nama: 'Halim Ngatidjan',
      jabatan: 'Executive Vice President',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        'Beliau memiliki pengalaman selama lebih dari 27 tahun di bidang keuangan, akuntansi, perpajakan, dan budgeting.',
      pendidikan:
        'Beliau meraih gelar Master of Business Administration dari Monash University, Melbourne pada tahun 1996.',
    },
    {
       warna: 'tabsec',
      id: 3,
      nama: 'Jahja Anwar',
      jabatan: 'Sekertaris Perusahaan',
      foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
      riwayat:
        'Country Manager di Wells Fargo Bank (2004-2012);• Executive Vice President di Perseroan (2012-2013) <br>• Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
      pendidikan:
        'Master of Business Adminstration (MBA) dari De Paul University Of Chicago, Amerika Serikat (1990).',
    },
  ],
});
</script>
