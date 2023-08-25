<template>
  <div class="flex py-12 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
     <div class="flex space-x-4 sm:justify-center">
      <div
        v-for="item in evp"
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
            bg-white/80
            translate-y-72
            sm:translate-y-64
            transition
            duration-300
            ease-in-out
            group-hover:-translate-y-0 group-hover:bg-white/80
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
  <div class="flex py-12 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
    <div class="flex space-x-4 sm:justify-center">
      <div
        v-for="item in komisaris"
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
          <div class="text-center">
            <h4 class="text-lg font-bold text-white">
              {{ item.nama }}
            </h4>
            <span class="block text-sm text-amber-300">{{ item.jabatan }}</span>
          </div>

          <p class="pt-3 mt-2 text-white text-xs w-full">
            <b>Riwayat:</b> <br />
        <p v-html="item.riwayat"></p>
          </p>
          <p class="pt-3 text-xs text-white">
            <b>Pendidikan:</b> <br />
        <p v-html="item.pendidikan"></p>
          </p>
        </div>
      </div>
    </div>
  </div>
    <div class="flex py-12 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
     <div class="flex space-x-4 sm:justify-center">
      <div
        class="
          group
          relative
          rounded-lg
          hover:shadow-xl
          w-72
          sm:w-1/4
          space-y-6
          overflow-hidden
          duration-200
        "
      >
<div class="bg-white p-4">
<div class="flex">
<p>TAHUN 2023</p>
<div class="flex"><p>TAHUN 2023</p> <p>TAHUN 2023</p></div>
</div></div>
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
    riwayat: 'Operation Director Tunas Toyota (2004-2006)<br>• Vice President di Tunas Toyota (2006-2010)<br>• Marketing and Sales Director di PT Mandiri Tunas Finance (2010-2021).',
    pendidikan: 'Sarjana Ekonomi dari Fakultas Ekonomi, Jurusan Manajemen, Universitas Krida Wacana Jakarta (1991)',
  },
  {
    nama: 'Engelbert Rorong, Jr.',
    jabatan: 'Direktur',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: '• Senior Manager di Perseroan (2006-2009)<br> • Executive Vice President di Perseroan (2009-2013)<br>• Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
    pendidikan: 'Beliau merupakan lulusan dari STIE PERBANAS, Jakarta (1992)',
  },
  {
    nama: 'Jahja Anwar',
    jabatan: 'Direktur',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Country Manager di Wells Fargo Bank (2004-2012);• Executive Vice President di Perseroan (2012-2013) <br>• Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
    pendidikan: 'Master of Business Adminstration (MBA) dari De Paul University Of Chicago, Amerika Serikat (1990).'
  },
  {
    nama: 'Yimmy Weddianto',
    jabatan: 'Direktur',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Area Manager di PT Nissan Motor Distributor Indonesia (2002-2005) <br>• Senior Vice President di PT Adira Dinamika Multifinance Tbk (2005-2016) <br>• Diangkat sebagai Direktur Perseroan sejak 2016.',
    pendidikan: 'Sarjana Teknik, Jurusan Teknik Industri dari Fakultas Teknik UniversitasTrisakti, Jakarta (2000).'
  },
];
const komisaris = [
  {
    nama: 'Roosniati Salihin',
    jabatan: 'Komisaris utama',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Memulai kariernya pada Divisi Internasional dan sebagai Executive Vice President di PT Bank Pan Indonesia Tbk (1991) sebelumnya Presiden Komisaris di PT Westpac Panin Bank (1991-1993)',
    pendidikan: '• Lulusan Bahasa Jepang dari Kokkusai Gakkuyukai, Tokyo, Jepang (1965) <br> • Lulusan English Literature dari University of California, Los Angeles, Amerika Serikat (1968)',
  },
  {
    nama: 'Bhindawati Gunawan',
    jabatan: 'Komisaris',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
     riwayat: '• Wakil Komisaris Utama PT Panin Financial Tbk (d/h PT Panin Life Tbk)(1991-2001) <br>• Menjabat sebagai Komisaris Utama Perusahaan (1991-2020) <br> dan • Menjabat sebagai Komisaris Perseroan (2020-sekarang)',
    pendidikan: 'Beliau merupakan lulusan Akademi Bisnis.',
  },
  {
    nama: 'Lukman Abdullah',
    jabatan: 'Komisaris Independen',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
  riwayat: '• Auditor di KAP Capelle Tuanakotta & Co. (1980-1990) <br> • Partner di KAP Drs. Hans Tuanakotta & Mustofa (1991-2002) <br> • Anggota Komite Audit di PT Asuransi Ramayana Tbk (2004-2008).',
    pendidikan: '• Sarjana Ekonomi dari Fakultas Ekonomi, Universitas Indonesia, Jakarta (1981)',
  },
];
const evp = [
  {
    nama: 'Donny Tri Wardono',
    jabatan: 'Executive Vice President',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Berbekal pengalaman lebih dari 27 tahun di bidang Sumber Daya Manusia (SDM), Beliau juga pernah menjabat posisi General Manager dan Senior General Manager di sejumlah perusahaan pembiayaan.',
    pendidikan: 'Beliau meraih gelar Sarjana (S1) dari Universitas Diponegoro, Semarang pada tahun 1985 dan gelar Magister (S2) dari Universitas Gadjah Mada, Jakarta pada tahun 2003.',
  },
  {
   nama: 'Halim Ngatidjan',
    jabatan: 'Executive Vice President',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Beliau memiliki pengalaman selama lebih dari 27 tahun di bidang keuangan, akuntansi, perpajakan, dan budgeting.',
    pendidikan: 'Beliau meraih gelar Master of Business Administration dari Monash University, Melbourne pada tahun 1996.'
  },
{
    nama: 'Jahja Anwar',
    jabatan: 'Sekertaris Perusahaan',
    foto: 'https://clipan.co.id/wp-content/uploads/2021/08/Har.png',
    riwayat: 'Country Manager di Wells Fargo Bank (2004-2012);• Executive Vice President di Perseroan (2012-2013) <br>• Menjabat sebagai Direktur Perseroan sejak tahun 2013.',
    pendidikan: 'Master of Business Adminstration (MBA) dari De Paul University Of Chicago, Amerika Serikat (1990).'
  },
];

const rups = [
  {
    tahun: '2023',
    icon: 'line-md:home-md-twotone',
    submenu: [{
      Juduls: 'profil perusahaan',
      iconmenu: 'solar:buildings-bold-duotone',
      deskripsi: 'konten berisikan tentang segala hal Clipan hal Clipan Finance',
      to: '/profil/tentang-perusahaan',
      daftarmenu: [{
        judul: 'Tentang Perusahaan',
        to: '/profile#tentang'
      },
      {
        judul: 'Visi Misi & Budaya',
        to: '/profile#visimisi'
      },
      {
        judul: 'Profile Manajemen',
        to: '/profile#vmanajemen'
      },
      {
        judul: 'Penghargaan & Struktur',
        to: '/profile#vmanajemen'
      }
      ]
    },
    {
      Juduls: 'tata kelola',
      iconmenu: 'solar:graph-new-up-bold-duotone',
      deskripsi: 'enghasilkan hasil yang sesuai dengan harapan pemangku kepentingan.',
      to: '/profil/tata-kelola',
      daftarmenu: [{
        judul: 'Pedoman Perusahaan',
        to: '/tata-kelola#tentang'
      },
      {
        judul: 'profesi penunjang',
        to: '/tata-kelola#visimisi'
      },
      {
        judul: 'Whistle blowing',
        to: '/tata-kelola#vmanajemen'
      },
      {
        judul: 'Anggaran dasar',
        to: '/tata-kelola#visimisi'
      }
      ]
    },
    {
      Juduls: 'hubungan investor',
      iconmenu: 'solar:round-sort-horizontal-bold-duotone',
      deskripsi: 'kami dapat senantiasa berkelanjutan dan menguntungkan.',
      to: '/profil/hubungan-investor',
      daftarmenu: [
        {
          judul: 'Informasi saham',
          to: '/tata-kelola#tentang'
        },
        {
          judul: 'Laporan Tahunan',
          to: '/tata-kelola#visimisi'
        },
        {
          judul: 'Laporan keuangan',
          to: '/tata-kelola#vmanajemen'
        },
        {
          judul: 'Prospektus',
          to: '/tata-kelola#visimisi'
        }

      ]
    },
    {
      Juduls: 'aksi korporasi',
      iconmenu: 'solar:cursor-square-bold-duotone',
      deskripsi: 'menciptakan inisiatif yang berdampak baik bagi masyarakat.',
      to: '/profil/aksi-korporasi',
      daftarmenu: [{
        judul: 'Karir',
        to: '/tata-kelola#tentang'
      },
      {
        judul: 'CSR',
        to: '/tata-kelola#visimisi'
      },
      {
        judul: 'Press Release',
        to: '/tata-kelola#vmanajemen'
      },
      {
        judul: 'Kegiatan',
        to: '/tata-kelola#visimisi'
      }
      ]
    }
    ]
  },
];
</script>
