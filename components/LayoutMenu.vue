<script setup>
import { ref } from 'vue';
import {
  Dialog,
  DialogPanel,
  Popover,
  PopoverButton,
  PopoverGroup,
  PopoverPanel,
  Tab,
  TabGroup,
  TabList,
  TabPanel,
  TabPanels,
  TransitionChild,
  TransitionRoot,
} from '@headlessui/vue';

const navigation = {
  categories: [
    {
      id: 'women',
      name: 'Women',
      featured: [
        {
          name: 'New Arrivals',
          href: '#',
          imageSrc:
            'https://tailwindui.com/img/ecommerce-images/mega-menu-category-01.jpg',
          imageAlt:
            'Models sitting back to back, wearing Basic Tee in black and bone.',
        },
        {
          name: 'Basic Tees',
          href: '#',
          imageSrc:
            'https://tailwindui.com/img/ecommerce-images/mega-menu-category-02.jpg',
          imageAlt:
            'Close up of Basic Tee fall bundle with off-white, ochre, olive, and black tees.',
        },
      ],
      sections: [
        {
          id: 'clothing',
          name: 'Clothing',
          items: [
            { name: 'Tops', href: '#' },
            { name: 'Dresses', href: '#' },
            { name: 'Pants', href: '#' },
            { name: 'Denim', href: '#' },
            { name: 'Sweaters', href: '#' },
            { name: 'T-Shirts', href: '#' },
            { name: 'Jackets', href: '#' },
            { name: 'Activewear', href: '#' },
            { name: 'Browse All', href: '#' },
          ],
        },
        {
          id: 'accessories',
          name: 'Accessories',
          items: [
            { name: 'Watches', href: '#' },
            { name: 'Wallets', href: '#' },
            { name: 'Bags', href: '#' },
            { name: 'Sunglasses', href: '#' },
            { name: 'Hats', href: '#' },
            { name: 'Belts', href: '#' },
          ],
        },
        {
          id: 'brands',
          name: 'Brands',
          items: [
            { name: 'Full Nelson', href: '#' },
            { name: 'My Way', href: '#' },
            { name: 'Re-Arranged', href: '#' },
            { name: 'Counterfeit', href: '#' },
            { name: 'Significant Other', href: '#' },
          ],
        },
      ],
    },
    {
      id: 'men',
      name: 'Men',
      featured: [
        {
          name: 'New Arrivals',
          href: '#',
          imageSrc:
            'https://tailwindui.com/img/ecommerce-images/product-page-04-detail-product-shot-01.jpg',
          imageAlt:
            'Drawstring top with elastic loop closure and textured interior padding.',
        },
        {
          name: 'Artwork Tees',
          href: '#',
          imageSrc:
            'https://tailwindui.com/img/ecommerce-images/category-page-02-image-card-06.jpg',
          imageAlt:
            'Three shirts in gray, white, and blue arranged on table with same line drawing of hands and shapes overlapping on front of shirt.',
        },
      ],
      sections: [
        {
          id: 'clothing',
          name: 'Clothing',
          items: [
            { name: 'Tops', href: '#' },
            { name: 'Pants', href: '#' },
            { name: 'Sweaters', href: '#' },
            { name: 'T-Shirts', href: '#' },
            { name: 'Jackets', href: '#' },
            { name: 'Activewear', href: '#' },
            { name: 'Browse All', href: '#' },
          ],
        },
        {
          id: 'accessories',
          name: 'Accessories',
          items: [
            { name: 'Watches', href: '#' },
            { name: 'Wallets', href: '#' },
            { name: 'Bags', href: '#' },
            { name: 'Sunglasses', href: '#' },
            { name: 'Hats', href: '#' },
            { name: 'Belts', href: '#' },
          ],
        },
        {
          id: 'brands',
          name: 'Brands',
          items: [
            { name: 'Re-Arranged', href: '#' },
            { name: 'Counterfeit', href: '#' },
            { name: 'Full Nelson', href: '#' },
            { name: 'My Way', href: '#' },
          ],
        },
      ],
    },
  ],
  pages: [
    { name: 'Company', href: '#' },
    { name: 'Stores', href: '/store' },
  ],
};

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

const open = ref(false);
</script>

<template>
  <div class="bg-white ">
    <!-- Mobile menu -->

    <header class="relative bg-white">
      <nav aria-label="Top" class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="border-b border-gray-200">
          <div class="flex h-16 items-center justify-between">
          
            <!-- Logo -->
            <div class="ml-4 flex lg:ml-0">
              <NuxtLink to="/">
                <span class="sr-only">Your Company</span>
                <img
                  class="h-8 w-auto"
                  src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600"
                  alt=""
                />
              </NuxtLink>
            </div>
            
            <!-- Flyout menus -->
            <PopoverGroup class=" lg:ml-8 lg:block lg:self-stretch">
              <div class="flex h-full space-x-8">
                <Popover
                  v-for="menu in nav"
                  :key="menu.judul"
                  v-slot="{ open }"
                  class="flex"
                >
                  <div class="relative flex">
                    <PopoverButton
                      class="
                        relative
                        z-10
                        -mb-px
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
                      <p class="font-bold uppercase text-xs sm:text-md  hover:text-blue-600">
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
                      class="absolute inset-x-0 top-full text-sm text-gray-500"
                    >
                      <div class="relative">
                        <div
                          class="
                            mx-auto
                            mt-2
                            max-w-screen-xl
                            bg-white
                            rounded-xl
                          "
                        >
                          <div
                            class="
                              p-8
                              grid grid-cols-2
                              sm:grid-cols-2
                              md:grid-cols-4
                            "
                          >
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
                                    <Icon
                                      name="uil:angle-right"
                                      class="w-3 h-3 mr-1"
                                    />
                                    <span :class="daftar.anime">
                                      {{ daftar.judul }}
                                      <Icon
                                        :name="daftar.promo"
                                        class="w-3 h-3 mr-1"
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
            </PopoverGroup>

            <div class="flex items-center">
              <NuxtLink to="/">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-6 h-6">
  <path d="M4.5 6.375a4.125 4.125 0 118.25 0 4.125 4.125 0 01-8.25 0zM14.25 8.625a3.375 3.375 0 116.75 0 3.375 3.375 0 01-6.75 0zM1.5 19.125a7.125 7.125 0 0114.25 0v.003l-.001.119a.75.75 0 01-.363.63 13.067 13.067 0 01-6.761 1.873c-2.472 0-4.786-.684-6.76-1.873a.75.75 0 01-.364-.63l-.001-.122zM17.25 19.128l-.001.144a2.25 2.25 0 01-.233.96 10.088 10.088 0 005.06-1.01.75.75 0 00.42-.643 4.875 4.875 0 00-6.957-4.611 8.586 8.586 0 011.71 5.157v.003z" />
</svg>

              </NuxtLink>
            </div>
          </div>
        </div>
      </nav>
    </header>
  </div>
</template>
