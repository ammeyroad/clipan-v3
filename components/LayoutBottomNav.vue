<template>
<div class="fixed bottom-0 left-0 z-50 w-full h-16 bg-white border-t border-gray-200 dark:bg-gray-700 dark:border-gray-600">
 <PopoverGroup class="">
    <div class="flex h-full space-x-8">
      <Popover
        v-for="menu in nav"
        :key="menu.judul"
        v-slot="{ open }"
        class="flex"
      >
        <div class="relative flex justify-beetwen">
          <PopoverButton
            class="
              relative
              z-10
              bg-b w-full
              flex
              items-center
              border-b-2
              pt-px
              text-sm
              font-medium
              transition-colors
              duration-200
              ease-out
            "
            :class="[
              open
                ? 'border-indigo-600 text-indigo-600 '
                : 'border-transparent text-gray-700 hover:text-gray-800',
            ]"
          >
            <Icon :name="menu.icon" class="w-6 h-6 mr-2" />
            <p
              class="font-bold uppercase text-xs sm:text-md hover:text-blue-600"
            >
              {{ menu.judul }}
            </p>
          </PopoverButton>
        </div>

        <transition
          enter-active-class="transition ease-out duration-200"
          enter-from-class="opacity-0"
          enter-to-class="opacity-100"
          leave-active-class="transition ease-in duration-150"
          leave-from-class="opacity-100"
          leave-to-class="opacity-0"
        >
          <PopoverPanel
            class="absolute text-sm text-gray-500"
          >
            <div class="relative bottom-0">
              <div class="mx-auto mt-2 max-w-screen-xl bg-white rounded-xl">
                <div class="p-8 grid grid-cols-2 sm:grid-cols-2 md:grid-cols-4">
                  <nuxtLink
                    v-for="sub in menu.submenu"
                    class="
                      flex flex-col
                      md:flex-row
                      h-60
                      md:gap-4
                      hover:bg-gray-100
                      rounded-lg
                      p-4
                    "
                    :href="'' + sub.to"
                  >
                    <div
                      class="
                        flex
                        h-12
                        w-12
                        shrink-0
                        items-center
                        justify-center
                        rounded-lg
                        md:h-10 md:w-10 md:rounded-xl
                      "
                    >
                      <Icon
                        :name="sub.iconmenu"
                        class="sm:w-12 sm:h-12 w-10 h-10"
                      />
                    </div>

                    <div class="mt-2 sm:mt-0">
                      <h3 class="font-extrabold text-lg capitalize">
                        {{ sub.Juduls }}
                      </h3>
                      <p class="sm:text-xs text-gray-500">
                        {{ sub.deskripsi }}
                      </p>

                      <ul
                        class="
                          space-y-1
                          hidden
                          sm:flex
                          flex-col
                          text-gray-500 text-sm
                        "
                      >
                        <hr class="my-2" />
                        <li
                          v-for="daftar in sub.daftarmenu"
                          :key="daftar.judul"
                          class="
                            text-sm
                            sm:text-md
                            hover:text-blue-600 hover:font-semibold
                            capitalize
                            items-center
                            duration-150
                          "
                        >
                          <Icon name="uil:angle-right" class="w-3 h-3 mr-1" />
                          <span :class="daftar.anime">
                            {{ daftar.judul }}
                            <Icon :name="daftar.promo" class="w-3 h-3 mr-1"
                          /></span>
                        </li>
                      </ul>
                    </div>
                  </nuxtLink>
                </div>
              </div>
            </div>
          </PopoverPanel>
        </transition>
      </Popover>
    </div>
  </PopoverGroup></div>
 
</template>

<script setup>
import { Popover, PopoverButton, PopoverPanel } from '@headlessui/vue';

const nav = [
  {
    judul: 'Profil',
    icon: 'line-md:home-md-twotone',
    submenu: [
      {
        Juduls: 'profil perusahaan',
        iconmenu: 'solar:buildings-bold-duotone',
        deskripsi:
          'konten berisikan tentang segala hal Clipan hal Clipan Finance',
        to: '/profil/tentang-perusahaan',
        daftarmenu: [
          {
            judul: 'Tentang Perusahaan',
            to: '/profile#tentang',
          },
          {
            judul: 'Visi Misi & Budaya',
            to: '/profile#visimisi',
          },
          {
            judul: 'Profile Manajemen',
            to: '/profile#vmanajemen',
          },
          {
            judul: 'Penghargaan & Struktur',
            to: '/profile#vmanajemen',
          },
        ],
      },
      {
        Juduls: 'tata kelola',
        iconmenu: 'solar:graph-new-up-bold-duotone',
        deskripsi:
          'enghasilkan hasil yang sesuai dengan harapan pemangku kepentingan.',
        to: '/profil/tata-kelola',
        daftarmenu: [
          {
            judul: 'Pedoman Perusahaan',
            to: '/tata-kelola#tentang',
          },
          {
            judul: 'profesi penunjang',
            to: '/tata-kelola#visimisi',
          },
          {
            judul: 'Whistle blowing',
            to: '/tata-kelola#vmanajemen',
          },
          {
            judul: 'Anggaran dasar',
            to: '/tata-kelola#visimisi',
          },
        ],
      },
      {
        Juduls: 'hubungan investor',
        iconmenu: 'solar:round-sort-horizontal-bold-duotone',
        deskripsi: 'kami dapat senantiasa berkelanjutan dan menguntungkan.',
        to: '/profil/hubungan-investor',
        daftarmenu: [
          {
            judul: 'Informasi saham',
            to: '/tata-kelola#tentang',
          },
          {
            judul: 'Laporan Tahunan',
            to: '/tata-kelola#visimisi',
          },
          {
            judul: 'Laporan keuangan',
            to: '/tata-kelola#vmanajemen',
          },
          {
            judul: 'Prospektus',
            to: '/tata-kelola#visimisi',
          },
        ],
      },
      {
        Juduls: 'aksi korporasi',
        iconmenu: 'solar:cursor-square-bold-duotone',
        deskripsi: 'menciptakan inisiatif yang berdampak baik bagi masyarakat.',
        to: '/profil/aksi-korporasi',
        daftarmenu: [
          {
            judul: 'Karir',
            to: '/tata-kelola#tentang',
          },
          {
            judul: 'CSR',
            to: '/tata-kelola#visimisi',
          },
          {
            judul: 'Press Release',
            to: '/tata-kelola#vmanajemen',
          },
          {
            judul: 'Kegiatan',
            to: '/tata-kelola#visimisi',
          },
        ],
      },
    ],
  },
  {
    judul: 'Produk',
    icon: 'line-md:bell-twotone',
    submenu: [
      {
        Juduls: 'Mobil baru',
        iconmenu: '',
        deskripsi: 'Mobil Baru kpm lorem ipsum dolremadsa sadsad',
        to: '/mobil-baru',
        daftarmenu: [
          {
            judul: 'KPM Panin',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/mobil-baru#',
          },
          {
            judul: 'Keungulan Produk',
            to: '/mobil-baru#',
          },
          {
            judul: 'Persyaratan Produk',
            to: '/mobil-baru',
          },
          {
            judul: 'Simulasi dan Pengajuan',
            to: '/mobil-baru#',
          },
        ],
      },
      {
        Juduls: 'Mobil Bekas',
        iconmenu: '',
        deskripsi: 'Mobil Bekas lorem ipsum dolremadsa sadsad',
        to: '/mobil-bekas',
        daftarmenu: [
          {
            judul: 'Keungulan Produk',
            to: '/mobil-bekas#',
          },
          {
            judul: 'Persyaratan Produk',
            to: '/mobil-bekas',
          },
          {
            judul: 'Pengajuan',
            to: '/mobil-bekas#',
          },
          {
            judul: 'Jaringan Digital',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/mobil-bekas#',
          },
        ],
      },
      {
        Juduls: 'Duit Cair',
        iconmenu: '',
        deskripsi: 'Dana Tunai as lorem ipsum dolremadsa sadsad',
        to: '/duit-cair',
        daftarmenu: [
          {
            judul: 'Keungulan Produk',
            to: '/duit-cair#',
          },
          {
            judul: 'Persyaratan Produk',
            to: '/duit-cair#',
          },
          {
            judul: 'Pengajuan',
            to: '/duit-cair#',
          },
          {
            judul: 'Peluang Bisnis',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/duit-cair#',
          },
        ],
      },
      {
        Juduls: 'Alat Berat & FLEET',
        iconmenu: '',
        deskripsi: 'Mobil Bekas lorem ipsum dolremadsa sadsad',
        to: '/alat-berat-fleet',
        daftarmenu: [
          {
            judul: 'Keungulan Produk',
            to: '/alat-berat-fleet',
          },
          {
            judul: 'Pengertian Fleet',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/alat-berat-fleet',
          },
          {
            judul: 'Jaringan & Perusahaan',
            to: '/alat-berat-fleet',
          },
        ],
      },
    ],
  },
  {
    judul: 'Layanan',
    icon: 'line-md:clipboard-arrow-twotone',
    submenu: [
      {
        Juduls: 'Layanan STNK',
        iconmenu: 'solar:pen-new-square-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/layanan',
        daftarmenu: [
          {
            judul: 'Perpanjang STNK',
            to: '/layanan#',
          },
          {
            judul: 'Kehilangan STNK',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
          {
            judul: 'Balik Nama Kendaraan',
            to: '/layanan#',
          },
          {
            judul: 'Artikel Terkait',
            to: '/layanan#',
          },
        ],
      },
      {
        Juduls: 'layanan BPKB',
        iconmenu: 'solar:book-bookmark-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/layanan',
        daftarmenu: [
          {
            judul: 'Informasi Umum',
            to: '/layanan#',
          },
          {
            judul: 'syarat Pengambilan',
            to: '/layanan#',
          },
          {
            judul: 'Tahap Pengambilan',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
          {
            judul: 'Artikel Terkait',
            to: '/layanan#',
          },
        ],
      },
      {
        Juduls: 'Bayaran Angsuran',
        iconmenu: 'solar:wallet-money-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/layanan',
        daftarmenu: [
          {
            judul: 'Informasi Umum',
            to: '/layanan#',
          },
          {
            judul: 'Melalui Bank Panin',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
          {
            judul: 'Melalui ATM Bersam',
            to: '/layanan#',
          },
          {
            judul: 'Indomaret dan Digital',
            to: '/layanan#',
          },
        ],
      },
      {
        Juduls: 'Layanan Pelangan',
        iconmenu: 'solar:shield-user-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/layanan',
        daftarmenu: [
          {
            judul: 'Cek Sisa Angsuran',
            to: '/layanan#',
          },
          {
            judul: 'Dokumen Kredit',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
          {
            judul: 'Janjian BPKB',
            to: '/layanan#',
          },
          {
            judul: 'Klaim asuransi',
            to: '/layanan#',
          },
        ],
      },
    ],
  },
  {
    judul: 'artikel',
    icon: 'line-md:text-box-multiple-twotone',
    submenu: [
      {
        Juduls: 'CLIMO',
        iconmenu: 'solar:file-download-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/berita',
        daftarmenu: [
          {
            judul: 'Clipan Mobile Apss',
            to: '/layanan#',
          },
          {
            judul: 'Informasi Climo',
            to: '/layanan#',
          },
          {
            judul: 'Keungulan CLimo',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
          {
            judul: 'Unduh Climo',
            to: '/layanan#',
          },
        ],
      },
      {
        Juduls: 'Berita Terbaru',
        iconmenu: 'solar:clipboard-heart-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/berita',
        daftarmenu: [
          {
            judul: 'Siaran resmi',
            to: '/layanan#',
          },
          {
            judul: 'produk',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
          {
            judul: 'Literasi',
            to: '/layanan#',
          },
          {
            judul: 'Layanan',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
        ],
      },
      {
        Juduls: 'promo Produk',
        iconmenu: 'solar:verified-check-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/berita',
        daftarmenu: [
          {
            judul: 'Mobil baru',
            to: '/layanan#',
          },
          {
            judul: 'mobil bekas',
            to: '/layanan#',
          },
          {
            judul: 'Duit cair',
            to: '/layanan#',
          },
          {
            judul: 'Promo GIIAS',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-600 font-bold',
            to: '/layanan#',
          },
        ],
      },
      {
        Juduls: 'Partnership',
        iconmenu: 'solar:case-bold-duotone',
        deskripsi: 'Lata lorem ipsum dolremadsa sadsad',
        to: '/berita',
        daftarmenu: [
          {
            judul: 'Carsome',
            to: '/layanan#',
          },
          {
            judul: 'Blibli',
            to: '/layanan#',
          },
          {
            judul: 'Lelang JBA',
            to: '/layanan#',
          },
          {
            judul: 'lihat Semua',
            to: '/layanan#',
          },
        ],
      },
    ],
  },
];
const solutions = [
  {
    name: 'Insights',
    description: 'Measure actions your users take',
    href: '##',
    icon: `
      <svg
        width="48"
        height="48"
        viewBox="0 0 48 48"
        fill="none"
        aria-hidden="true"
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect width="48" height="48" rx="8" fill="#FFEDD5" />
        <path
          d="M24 11L35.2583 17.5V30.5L24 37L12.7417 30.5V17.5L24 11Z"
          stroke="#FB923C"
          stroke-width="2"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M16.7417 19.8094V28.1906L24 32.3812L31.2584 28.1906V19.8094L24 15.6188L16.7417 19.8094Z"
          stroke="#FDBA74"
          stroke-width="2"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M20.7417 22.1196V25.882L24 27.7632L27.2584 25.882V22.1196L24 20.2384L20.7417 22.1196Z"
          stroke="#FDBA74"
          stroke-width="2"
        />
      </svg>
    `,
  },
  {
    name: 'Automations',
    description: 'Create your own targeted content',
    href: '##',
    icon: `
      <svg
        width="48"
        height="48"
        viewBox="0 0 48 48"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect width="48" height="48" rx="8" fill="#FFEDD5" />
        <path
          d="M28.0413 20L23.9998 13L19.9585 20M32.0828 27.0001L36.1242 34H28.0415M19.9585 34H11.8755L15.9171 27"
          stroke="#FB923C"
          stroke-width="2"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M18.804 30H29.1963L24.0001 21L18.804 30Z"
          stroke="#FDBA74"
          stroke-width="2"
        />
      </svg>
    `,
  },
  {
    name: 'Reports',
    description: 'Keep track of your growth',
    href: '##',
    icon: `
      <svg
        width="48"
        height="48"
        viewBox="0 0 48 48"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect width="48" height="48" rx="8" fill="#FFEDD5" />
        <rect x="13" y="32" width="2" height="4" fill="#FDBA74" />
        <rect x="17" y="28" width="2" height="8" fill="#FDBA74" />
        <rect x="21" y="24" width="2" height="12" fill="#FDBA74" />
        <rect x="25" y="20" width="2" height="16" fill="#FDBA74" />
        <rect x="29" y="16" width="2" height="20" fill="#FB923C" />
        <rect x="33" y="12" width="2" height="24" fill="#FB923C" />
      </svg>
    `,
  },
];
</script>
