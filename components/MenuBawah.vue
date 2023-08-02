<template>
  <div class="grid grid-cols-4 w-full fixed bottom-0 bg-white rounded-t-xl">
    <div v-for="team in teams" :key="team.id" class="flex-col text-center py-2">
      <button class="text-sm hover:text-blue-600" @click="openModal(team.judul)">
       <div class=" w-max mx-auto">
        <Icon :name="team.icon" class="w-6 h-6" />
        <p class="font-bold  uppercase text-xs sm:text-md">
          {{ team.judul }}
        </p>
      </div>
      </button>
    </div>

    <transition name="modal">
      <div v-if="isModalOpen" class="modal-overlay">
        <div class="modal-container">
          <div class="modal-content grid grid-cols-2">
            <button class="btn-b w-max col-span-2" @click="closeModal">
              tutup
            </button>
            <nuxtLink
              v-for="sub in selectedUser.submenu"
              class="
                flex flex-col
                md:flex-row
                h-48
                sm:h-60
                md:gap-4
                hover:bg-gray-100
                rounded-lg
                p-2
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
                <Icon :name="sub.iconmenu" class="sm:w-12 sm:h-12 w-10 h-10" />
              </div>

              <div class="mt-2 sm:mt-0">
                <h3 class="text-lg font-semibold capitalize">
                  {{ sub.Juduls }}
                </h3>
                <p class="text-xs text-gray-500">
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
    </transition>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const teams = [
  {
    id: 3,
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
    id: 3,
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
    id: 3,
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
    id: 3,
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

const isModalOpen = ref(false);
const selectedUser = ref(null);

const openModal = (judul) => {
  isModalOpen.value = true;
  // Temukan pengguna yang dipilih berdasarkan judul
  selectedUser.value = teams.find((team) => team.judul === judul);
};

const closeModal = () => {
  isModalOpen.value = false;
  selectedUser.value = null;
};

const closeModalOutside = (event) => {
  if (!event.target.closest('.modal-content')) {
    closeModal();
  }
};
</script>

<style>
.card {
  @apply py-2 px-4 mb-2 border rounded;
}

.username-btn {
  @apply bg-blue-500 text-white border-none px-4 py-2 cursor-pointer;
}

.modal-overlay {
  @apply fixed bottom-16  w-full  flex;
}

.modal-container {
  @apply rounded;
}

.modal-content {
  @apply bg-white  p-4;
}
</style>
