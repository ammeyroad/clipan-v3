<template>
  <section class="relative py-12 dark:bg-jacarta-800">
    <div class="max-w-screen-lg mx-auto pl-4">
      <div class="sm:text-center text-left">
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

        <h3 class="text-blue-600 text-2xl pt-2 font-extrabold md:text-4xl">
          Inilah Tujuan Kita Sebenarnya
        </h3>
        <garis />

        <p class="pr-8 sm:px-32 pb-5">
          Berawal dari marketplace lalu tumbuh menjadi platform yang memberikan
          banyak kemudahan untuk berbisnis. Inilah kami,
        </p>
      </div>
      <div class="grid grid-cols-2">
      <div>aaa</div>
      <div>222</div>
      </div>
    </div>
  </section>
</template>

<script setup>
const steps = [
  {
    tanggal: '15 Januari',
    tahun: '1982',
    konten: 'Berdiri dengan nama PT Clipan Leasing Corporation',
  },
  {
    tanggal: '17 Mei',
    tahun: '1990',
    konten: 'Perubahan nama menjadi PT Clipan Finance Indonesia',
  },
  {
    tanggal: '27 Agustus',
    tahun: '1990',
    konten: 'Resmi melakukan penawaran saham perdana di BEJ',
  },
  {
    tanggal: '30 Agustus',
    tahun: '1990',
    konten: 'Berganti nama menjadi PT Clipan Finance Indonesia Tbk',
  },
];
</script>
