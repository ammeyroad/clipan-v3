<template>
  <div class="grid content-center z-20 sm:inset-0 mx-auto sm:top-0 left-0 w-max">
    <button v-for="menu in nav" type="button" class="bg-gray-100 hover:bg-blue-600 font-medium rounded-xl text-sm p-1.5 text-center inline-flex items-center text-blue-600 hover:text-white group">
      <div class=" w-max mx-auto">
        <Icon name="solar:call-chat-rounded-bold-duotone" class="w-8 h-8 p-1" />
      </div>
      <div class="hidden z-50 group-hover:grid h-max fixed top-14 sm:pt-8 max-w-screen-xl inset-0 w-full p-2 sm:px-0 mx-auto place-content-end">
        <div class=" grid place-content-end ">
          <div class="text-left p-2 bg-white rounded-lg sm:shadow-xl ">
            <nuxtLink v-for="sub in menu.submenu" class="flex gap-2 text-gray-700 hover:bg-gray-100 hover:text-blue-600 rounded-lg p-2 items-center" :href="'' + sub.to">
              <div class="flex h-8 w-8 shrink-0 items-center justify-center rounded-lg md:h-10 md:w-10 md:rounded-xl">
                <Icon :name="sub.iconmenu" class=" w-8 h-8" />
              </div>
              <p class="text-sm font-semibold capitalize ">
                {{ sub.Juduls }}
              </p>
            </nuxtLink>
          </div>
        </div>
      </div>
    </button>
  </div>
</template>

<script setup>
const nav = [{
  icon: 'line-md:home-md-twotone',
  submenu: [{
    Juduls: 'Pengaduan Konsumen',
     iconmenu: 'solar:letter-unread-bold-duotone',
    deskripsi: 'konten berisikan tentang segala hal Clipan hal Clipan Finance',
    to: '/profil/tentang-perusahaan'
  },
  {
    Juduls: 'Kantor Cabang',
     iconmenu: 'solar:point-on-map-bold-duotone',
    deskripsi: 'enghasilkan hasil yang sesuai dengan harapan pemangku kepentingan.',
    to: '/profil/tata-kelola'
  },
  {
    Juduls: 'Whatsapp Bot',
     iconmenu: 'solar:chat-round-unread-bold-duotone',
    deskripsi: 'kami dapat senantiasa berkelanjutan dan menguntungkan.',
    to: '/profil/hubungan-investor'
  },
  {
    Juduls: 'Cek Pengajuan',
     iconmenu: 'solar:bell-bing-bold-duotone',
    deskripsi: 'menciptakan inisiatif yang berdampak baik bagi masyarakat.',
    to: '/profil/aksi-korporasi'
  }
  ]
}
]
</script>
