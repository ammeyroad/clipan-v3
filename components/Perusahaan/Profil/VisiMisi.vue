<template>
  <section class="py-24 bg-white">
    <div class="max-w-screen-lg mx-auto px-4">
      <div class="sm:text-center text-left mb-10">
        <div
          class="
            inline-flex
            justify-between
            items-center
            py-1
            px-1
            text-sm text-gray-700
            bg-white
            rounded-full
          "
          role="alert"
        >
          <span
            class="
              text-xs
              bg-yellow-400
              rounded-full
              text-black
              font-semibold
              px-4
              py-1.5
              mr-3
            "
            >Visi Misi</span
          >
          <span class="text-sm font-medium mr-2">dan Budaya</span>
        </div>

        <h3 class="">Inilah Tujuan Kita Sebenarnya</h3>
        <garis />

        <p class="pr-8 sm:px-32 pb-5">
          Berawal dari marketplace lalu tumbuh menjadi platform yang memberikan
          banyak kemudahan untuk berbisnis. Inilah kami,
        </p>
      </div>
      <div class="grid sm:grid-cols-5 gap-10">
        <div class="sm:col-span-2">
          <div
            class="
              mx-auto
              max-w-screen-lg
              rounded-xl
              p-6
              border-2 border-yellow-400
              bg-gradient-to-br
              from-yellow-400
              to-yellow-500
              shadow-md
            "
          >
            <h3>Visi</h3>
            <p class="text-justify mt-2">
              Menjadi perusahaan pembiayaan terkemuka yang mengedepankan nilai
              tambah bagi pemangku kepentingan dan berperan aktif dalam
              pertumbuhan industri pembiayaan nasional.
            </p>
            <hr class="border-black opacity-50 my-6" />
            <h3>Misi</h3>
            <div class="grid gap-5">
              <div class="flex items-top">
                <Icon
                  name="solar:round-alt-arrow-right-bold"
                  class="w-12 mt-1 mr-2"
                />
                <p class="text-justify">
                  Menyediakan produk dan jasa keuangan yang inovatif didukung
                  sumber daya manusia yang handal dan teknologi terkini.
                </p>
              </div>
              <div class="flex items-top">
                <Icon
                  name="solar:round-alt-arrow-right-bold"
                  class="w-10 mt-1 mr-2"
                />
                <p class="text-justify">
                  Mempertahankan dan meningkatkan kinerja keuangan yang sehat
                  dan berkelanjutan.
                </p>
              </div>
              <div class="flex items-top">
                <Icon
                  name="solar:round-alt-arrow-right-bold"
                  class="w-10 mt-1 mr-2"
                />
                <p class="text-justify">
                  Menjalankan perusahaan sesuai dengan prinsip-prinsip tata
                  kelola perusahaan yang baik.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="sm:col-span-3">
          <h3>Budaya Perusahaan</h3>
          <p class="text-justify">
            Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola
            perusahaan yang baik.
          </p>

          <div class="grid">
            <div v-for="item in budaya" class="hover:bg-white rounded-xl sm:p-3 p-4 flex">
              <h4 class=" lowercase">
                <span
                  class="p-1 bg-blue-600 px-3 rounded text-white uppercase"
                  >{{ item.inisial }}</span
                >
              </h4>
              <div>
                <h4 class="ml-1 lowercase">{{ item.judul }}</h4>
                <p class="ml-2 text-gray-500 dark:text-gray-400 text-justify">
                 {{ item.isi }}
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const budaya = [
  {
    inisial: 'C',
    judul: 'reative',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik.',
  },
  {
    inisial: 'L',
    judul: 'iga',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik.',
  },
  {
    inisial: 'I',
    judul: 'ntegrity',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik.',
  },
  {
    inisial: 'P',
    judul: 'rofesional',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik.',
  },
  {
    inisial: 'FUN',
    judul: 'ergic',
    isi: 'Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola perusahaan yang baik.',
  },
];
</script>
