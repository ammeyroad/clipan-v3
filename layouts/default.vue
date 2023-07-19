<template>
  <main class="">
<nav class="fixed w-full z-20 top-0 left-0">
    <div class="max-w-screen-xl sm:mt-2 bg-white sm:rounded-xl flex items-center justify-between mx-auto sm:p-4 p-2 shadow-xl">
      <a href="/" class="flex items-center">
        <img src="/clipan-logo.png" class="h-8">
      </a>
      <div class="flex md:order-2 gap-2">
        <MenuCari />
        <MenuCS />
      </div>
      <MenuNav />
    </div>
  </nav>
    <slot />

    <div class="pt-12 lg:pt-16 bg-blue-600 text-white">
      <div class="mx-auto max-w-screen-xl">
        <div class="mx-auto max-w-screen-2xl px-4 md:px-8">
          <div class="mb-16 grid grid-cols-2 gap-2 md:grid-cols-5 lg:gap-4">
            <div class="p-2 col-span-2">
              <!-- logo - start -->
              <div class="mb-4 lg:-mt-2">
                <a
                  href="/"
                  class="
                    text-black-800
                    inline-flex
                    items-center
                    gap-2
                    text-xl
                    font-bold
                    md:text-2xl
                  "
                  aria-label="logo"
                >
                  <svg
                    width="95"
                    height="94"
                    viewBox="0 0 95 94"
                    class="h-auto w-5 text-indigo-500"
                    fill="currentColor"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path d="M96 0V47L48 94H0V47L48 0H96Z" />
                  </svg>

                  Clipan Finance Indonesia
                </a>
              </div>
              <!-- logo - end -->

              <p class="mb-6 sm:pr-8">
                Filler text is dummy text which has no meaning however looks
                very similar to real text
              </p>

              <!-- social - start -->
              <div class="flex gap-4">
                <a
                  href="#"
                  target="_blank"
                  class="
                    text-gray-400
                    transition
                    duration-100
                    hover:
                    active:text-gray-600
                  "
                >
                  <svg
                    class="h-5 w-5"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"
                    />
                  </svg>
                </a>

                <a
                  href="#"
                  target="_blank"
                  class="
                    text-gray-400
                    transition
                    duration-100
                    hover:
                    active:text-gray-600
                  "
                >
                  <svg
                    class="h-5 w-5"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"
                    />
                  </svg>
                </a>

                <a
                  href="#"
                  target="_blank"
                  class="
                    text-gray-400
                    transition
                    duration-100
                    hover:
                    active:text-gray-600
                  "
                >
                  <svg
                    class="h-5 w-5"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"
                    />
                  </svg>
                </a>

                <a
                  href="#"
                  target="_blank"
                  class="
                    text-gray-400
                    transition
                    duration-100
                    hover:
                    active:text-gray-600
                  "
                >
                  <svg
                    class="h-5 w-5"
                    width="24"
                    height="24"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"
                    />
                  </svg>
                </a>
              </div>
              <!-- social - end -->
            </div>

            <!-- nav - start -->
            <div class="p-5 hover:bg-black/20 rounded-xl duration-300">
              <div class="bg-black/10 p-3 rounded-lg w-12 h-12 mb-2">
                <Icon
                  name="heroicons-outline:phone-incoming"
                  class="w-6 h-6 mr-2"
                />
              </div>
              <h1 class="font-black">1500 333</h1>
              <h1 class="font-semibold tracking-tighter mt-4">Telepon</h1>
              <p class="mx-auto text-xs">Senin – Jumat, 08.30-16.00</p>
            </div>
            <!-- nav - end -->

            <!-- nav - start -->
            <div class="p-5 hover:bg-black/20 rounded-xl duration-300">
              <div class="bg-black/10 p-3 rounded-lg w-12 h-12 mb-2">
                <Icon name="heroicons-outline:envelope" class="w-6 h-6 mr-2" />
              </div>
              <h1 class="font-black">cs@clipan.co.id</h1>
              <h1 class="font-semibold tracking-tighter mt-4">Email</h1>
              <p class="mx-auto text-xs">Senin – Jumat, 08.30-16.00</p>
            </div>
            <!-- nav - end -->

            <!-- nav - start -->
            <div class="p-5 hover:bg-black/20 rounded-xl duration-300">
              <div class="bg-black/10 p-3 rounded-lg w-12 h-12 mb-2">
                <Icon name="heroicons-outline:map-pin" class="w-6 h-6 mr-2" />
              </div>
              <h1 class="font-black">Lihat Cabang</h1>
              <h1 class="font-semibold tracking-tighter mt-4">Jam Layanan</h1>
              <p class="mx-auto text-xs">Senin – Jumat, 08.30-16.00</p>
            </div>
          </div>

          <div
            class="
              bg-black/20
              rounded-t-lg
              py-8
              text-center text-sm text-gray-400
            "
          >
            © 2021 - Present Flowrift. All rights reserved.
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
            to: '/layanan#',
          },
          {
            judul: 'Literasi',
            to: '/layanan#',
          },
          {
            judul: 'Layanan',
            promo: 'ic:twotone-thumb-up',
            anime: 'animate-pulse text-blue-400 font-bold',
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
            anime: 'animate-pulse text-blue-400 font-bold',
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
</script>
