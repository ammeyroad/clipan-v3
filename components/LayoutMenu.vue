<template>
    <nav class="fixed w-full z-20 top-0 left-0">
      <div
        class="
          max-w-screen-xl
          sm:mt-2
          bg-white
          sm:rounded-xl
          flex
          items-center
          justify-between
          mx-auto
          sm:p-4
          p-2
          shadow-xl
        "
      >
        <a href="/" class="flex items-center">
          <img src="/clipan-finance-logo.svg" class="h-8" />
        </a>
        <div class="flex md:order-2 gap-2 sticky top-0">
          <MenuCari />
          <MenuCS />
        </div>
        <MenuNav />
      </div>
    </nav>
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