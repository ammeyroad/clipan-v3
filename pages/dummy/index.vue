<template>
  <div>
    <section>
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
          <div class="mb-2">
            <span
              class="inline-block w-12 h-1.5 bg-blue-500 rounded-full"
            ></span
            ><span
              class="inline-block w-4 h-1.5 ml-1 bg-yellow-400 rounded-full"
            ></span
            ><span
              class="inline-block w-1.5 h-1.5 ml-1 bg-yellow-400 rounded-full"
            ></span>
          </div>
          <h3 class="pr-8 sm:px-32 hed4 normal-case">
            Kinerja Clipan tidak lepas dari peranan jajaran Komisaris dan
            Direksi yang berpengalaman, berprestasi, dan pakar di bidangnya.
          </h3>
        </div>
        <div class="w-full mx-auto max-w-screen-lg sm:px-0">
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
                      ? 'bg-blue-600 text-white shadow'
                      : 'text-gray-600 font-bold hover:bg-white/[0.12] hover:text-blue-600',
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
                  class="
                    flex
                    w-full
                    md:mx-auto md:max-w-screen-xl
                    overflow-x-auto
                  "
                >
                  <div class="flex space-x-4 sm:justify-center">
                    <div
                      v-for="post in posts"
                      :key="post.id"
                      class="
                        mb-8
                        group
                        relative
                        rounded-xl
                        shadow-lg
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
                          sm:h-full
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
                          <div class="rounded-lg my-1">
                            <h5 class="text-xl font-bold">
                              {{ post.nama }}
                            </h5>
                            <span class="block text-sm">{{
                              post.jabatan
                            }}</span>
                          </div>
                          <div class="text-left pt-3 w-full p-2">
                            <p class="text-sm font-bold">Riwayat</p>
                            <p class="text-xs mb-2" v-html="post.riwayat"></p>
                            <p class="text-sm font-bold">Pendidikan</p>
                            <p
                              class="text-xs mb-2"
                              v-html="post.pendidikan"
                            ></p>
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
      </div>
    </section>

    <section class="bg-white pt-96 -mt-72 py-24">
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
            >Investor dan Korporasi</span
          >
          <h1 class="hed3 mt-4">Informasi RUPS dan Berita lainnya</h1>
          <div class="mb-2">
            <span
              class="inline-block w-12 h-1.5 bg-blue-500 rounded-full"
            ></span
            ><span
              class="inline-block w-4 h-1.5 ml-1 bg-yellow-400 rounded-full"
            ></span
            ><span
              class="inline-block w-1.5 h-1.5 ml-1 bg-yellow-400 rounded-full"
            ></span>
          </div>
          <h3 class="pr-8 sm:px-32 pb-5 hed4">
            Informasi bagi investor, masyarakat pasar modal dan pemegang saham
            disajikan dengan transparan
          </h3>
        </div>
        <div class="flex w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
          <div class="flex sm:flex-wrap">
            <div v-for="daftar in rups" class="px-2 pb-6 sm:px-4 w-72 sm:w-1/2">
              <div
                class="
                  rounded-xl
                  hover:shadow-lg
                  bg-white
                  border border-blue-50
                  hover:bg-gray-50
                  rounded-xl
                  duration-200
                "
              >
                <div class="">
                  <h4
                    class="
                      uppercase
                      text-white
                      rounded-t-xl
                      bg-blue-600
                      text-2xl
                      font-bold
                      text-center
                      p-4
                    "
                  >
                    {{ daftar.tahun }}
                  </h4>
                </div>
                <ul class="divide-y divide-gray-300/50 p-2">
                  <li
                    v-for="link in daftar.daftars"
                    class="
                      flex
                      items-center
                      px-4
                      py-2
                      justify-between
                      group
                      hover:bg-white hover:shadow-md
                      rounded-lg
                      duration-200
                    "
                  >
                    <p
                      class="
                        group-hover:font-bold group-hover:text-blue-600
                        duration-200
                        capitalize
                      "
                    >
                      {{ link.judul }}
                    </p>

                    <div class="flex">
                      <a
                        v-for="file in link.download"
                        :href="file.to"
                        class="
                          opacity-50
                          group-hover:opacity-100
                          scale-75
                          fill-gray-400
                          group-hover:scale-100
                          duration-200
                          hover:animate-bounce hover:fill-blue-600
                        "
                        ><svg
                          xmlns="http://www.w3.org/2000/svg"
                          width="32"
                          height="32"
                          viewBox="0 0 24 24"
                        >
                          <path
                            fill-rule="evenodd"
                            d="M2 12c0-4.714 0-7.071 1.464-8.536C4.93 2 7.286 2 12 2c4.714 0 7.071 0 8.535 1.464C22 4.93 22 7.286 22 12c0 4.714 0 7.071-1.465 8.535C19.072 22 16.714 22 12 22s-7.071 0-8.536-1.465C2 19.072 2 16.714 2 12Zm10-5.75a.75.75 0 0 1 .75.75v5.19l1.72-1.72a.75.75 0 1 1 1.06 1.06l-3 3a.75.75 0 0 1-1.06 0l-3-3a.75.75 0 1 1 1.06-1.06l1.72 1.72V7a.75.75 0 0 1 .75-.75Zm-4 10a.75.75 0 0 0 0 1.5h8a.75.75 0 0 0 0-1.5H8Z"
                            clip-rule="evenodd"
                          />
                        </svg>
                      </a>
                    </div>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue';
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

const rups = [
  {
    tahun: '2023 Luar Biasa',
    daftars: [
      {
        judul: 'Pengumuman',
        download: [
          {
            to: '/2023-2-RUPSLB-PENGUMUMAN.pdf',
          },
        ],
      },
      {
        judul: 'Pemanggilan',
        download: [
          {
            to: '/2023-2-RUPSLB-PEMANGGILAN.pdf',
          },
        ],
      },
      {
        judul: 'Tata Tertib',
        download: [
          {
            to: '/2023-2-RUPSLB-TATATERTIB.pdf',
          },
        ],
      },
      {
        judul: 'Surat Kuasa',
        download: [
          {
            to: '/2023-2-RUPSLB-SURATKUASA.pdf',
          },
        ],
      },
            {
        judul: 'Risalah Rapat',
        download: [
          {
            to: '/2023-2-RUPSLB-RISALAH.pdf',
          },
        ],
      },
    ],
  },
  {
    tahun: 'Tahun 2023',
    daftars: [
      {
        judul: 'Pengumuman',
        download: [
          {
            to: '/2023-PENGUMUMAN-ID.pdf',
          },
        ],
      },
      {
        judul: 'Pemanggilan',
        download: [
          {
            to: '/2023-PEMANGGILAN-ID.pdf',
          },
        ],
      },
      {
        judul: 'Tata Tertib',
        download: [
          {
            to: '/2023-TATATERTIB-ID.pdf',
          },
        ],
      },
      {
        judul: 'Surat Kuasa',
        download: [
          {
            to: '/2023-SURATKUASA-ID.pdf',
          },
        ],
      },
       {
        judul: 'Risalah Rapat',
        download: [
          {
            to: '/2023-RISALAH-ID.pdf',
          },
        ],
      },
      {
        judul: 'Materi',
        download: [
          {
            to: '/2023-MATERI.pdf',
          },
        ],
      },
    ],
  },
  {
    tahun: 'TAHUN 2022',
    daftars: [
      {
        judul: 'Pengumuman',
        download: [
          {
            to: '/2022-PENGUMUMAN-ID.pdf',
          },
           {
            to: '/2022-PENGUMUMAN-ENG.pdf',
          },
        ],
      },
            {
        judul: 'Pemanggilan',
        download: [
          {
            to: '/2023-PEMANGGILAN-ID.pdf',
          },
          {
            to: '/2023-PEMANGGILAN-EN.pdf',
          },
        ],
      },
      {
        judul: 'Tata Tertib',
        download: [
          {
            to: '/2022-TATATERTIB.pdf',
          },
        ],
      },
      {
        judul: 'Surat Kuasa',
        download: [
          {
            to: '/2022-SURATKUASA.pdf',
          },
        ],
      },
      {
        judul: 'Risalah Rapat',
        download: [
          {
            to: '/2022-RISALAH-ID.pdf',
          },
           {
            to: '/2022-RISALAH-ENG.pdf',
          },
        ],
      },
    ],
  },
];

const categories = ref({
  KOMISARIS: [
    {
      id: 1,
      warna: 'tabkomisaris',
      nama: 'Roosniati Salihin',
      jabatan: 'Komisaris utama',
      foto: 'https://clipan.id/aset/uploads/Manajemen-Roosmiati.jpg',
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
      foto: 'https://clipan.id/aset/uploads/Manajemen-Bhinda.jpg',
      riwayat:
        '• Wakil Komisaris Utama PT Panin Financial Tbk (d/h PT Panin Life Tbk)(1991-2001) <br>• Menjabat sebagai Komisaris Utama Perusahaan (1991-2020) <br> dan • Menjabat sebagai Komisaris Perseroan (2020-sekarang)',
      pendidikan: 'Beliau merupakan lulusan Akademi Bisnis.',
    },
    {
      warna: 'tabkomisaris',
      id: 3,
      nama: 'Lukman Abdullah',
      jabatan: 'Komisaris Independen',
      foto: 'https://clipan.id/aset/uploads/Manajemen-Lukman.jpg',
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
      foto: 'https://clipan.id/aset/uploads/Manajemen-Hartjanto.jpg',
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
      foto: 'https://clipan.id/aset/uploads/Manajemen-Jahja.jpg',
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
      foto: 'https://clipan.id/aset/uploads/Manajemen-engelbert.jpg',
      riwayat:
        '• Senior Manager di Perseroan (2006-2009)<br> • Executive Vice President di Perseroan (2009-2013)<br> • Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
      pendidikan: 'Beliau merupakan lulusan dari STIE PERBANAS, Jakarta (1992)',
    },
    {
      warna: 'tabdireksi',
      id: 4,
      nama: 'Yimmy Weddianto',
      jabatan: 'Direktur',
      foto: 'https://clipan.id/aset/uploads/Manajemen-Yimmy.jpg',
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
      foto: 'https://clipan.id/aset/uploads/Manajemen-Donny.jpg',
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
      foto: 'https://clipan.id/aset/uploads/Manajemen-Halim.jpg',
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
      foto: 'https://clipan.id/aset/uploads/Manajemen-Jahja.jpg',
      riwayat:
        'Country Manager di Wells Fargo Bank (2004-2012);• Executive Vice President di Perseroan (2012-2013) <br>• Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
      pendidikan:
        'Master of Business Adminstration (MBA) dari De Paul University Of Chicago, Amerika Serikat (1990).',
    },
  ],
});
</script>
