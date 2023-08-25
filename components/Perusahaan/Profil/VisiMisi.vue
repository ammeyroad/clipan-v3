<template>
  <section class="py-24 bg-white">
    <div class="max-w-screen-lg mx-auto px-4">
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
          >Visi, Misi dan Budaya</span
        >

        <h1 class="hed3 mt-4">Tujuan Clipan dan budaya kerja</h1>
        <garis />

        <h3 class="sm:px-32 pb-5 hed4">
          Berawal dari marketplace lalu tumbuh menjadi platform yang memberikan
          banyak kemudahan untuk berbisnis. Inilah kami,
        </h3>
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
            <h3 class="text-black">Visi</h3>
            <p class="text-justify mt-2">
              Menjadi perusahaan pembiayaan terkemuka yang mengedepankan nilai
              tambah bagi pemangku kepentingan dan berperan aktif dalam
              pertumbuhan industri pembiayaan nasional.
            </p>
            <hr class="border-black opacity-50 my-6" />
            <h3 class="text-black">Misi</h3>
            <div class="grid gap-5 mt-2">
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
          <h4 class="text-xl uppercase">Budaya Perusahaan</h4>
          <p class="text-justify">
            Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola
            perusahaan yang baik.
          </p>

          <div class="pt-5">
            <div 
              v-for="item in budaya"
            >
              <div class="grid grid-cols-8 border-b-2 border-white items-center">
                <h3 class="bg-blue-100 grid items-center text-center break-all px-2 sm:px-4 py-2 h-full"> {{ item.inisial }}</h3>
                <div class="col-span-7 p-2">
                  <h3 class="hed4 uppercase">{{ item.judul }}</h3>
                  <p class="text-sm">
                    {{ item.isi }}
                  </p>
                </div>
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
