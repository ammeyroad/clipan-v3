<template>
    <section class="relative py-12 dark:bg-jacarta-800">
      <div class="max-w-screen-lg mx-auto pl-4">
        <div class="sm:text-center text-left pl-2">
          <p class="font-semibold text-yellow-500 text-sm xl:text-xl"></p>
          <span
            class="
              bg-yellow-400
              text-black text-xs
              font-medium
              mr-2
              px-2.5
              py-1.5
              rounded-xl
            "
            >Sejarah Singkat</span
          >
          <h3 class="hed3">Clipan Finance Indonesia</h3>
          <garis />
        </div>
        <p class="text-justify pr-6 pl-2 ">
          Clipan Finance adalah bagian dari Panin Group, perusahaan dengan
          pengalaman sejak 1982 di industri pembiayaan. Fokus utama kami adalah
          memberikan pembiayaan untuk mobil baru, mobil bekas, alat berat, dan
          multiguna. Visi kami adalah menjadi perusahaan pembiayaan terkemuka
          yang membantu masyarakat Indonesia mencapai impian mereka. Kami
          menawarkan pelayanan terbaik dan solusi finansial yang tepat sesuai
          kebutuhan pelanggan.
          <br /><br />
          PT Clipan Finance Indonesia Tbk (“Perseroan”) pertama kali didirikan
          dengan nama PT Clipan Leasing Corporation berdasarkan Akta No. 47 pada
          15 Januari 1982 yang dibuat dihadapan Kartini Muljadi, S.H., Notaris
          di Jakarta. Dalam tonggak sejarah berikutnya, tepatnya pada 17 Mei
          1990, Perseroan melakukan perubahan nama dari semula PT Clipan Leasing
          Corporation menjadi PT Clipan Finance Indonesia yang mana perubahan
          tersebut mengacu pada Akta No. 56 tanggal 17 Mei 1990 dan telah
          disahkan melalui Surat Keputusan Menteri Kehakiman Republik Indonesia
          No. C2.3418.HT.01.04.th 90 tanggal 5 Juli 1990.
        </p>
        <div
          class="
            flex
            py-12
            w-full
            md:mx-auto md:max-w-screen-xl
            overflow-x-auto
          "
        >
          <div class="flex space-x-4">
            <div
              v-for="step in steps"
              class="
                w-52
                sm:w-1/4
                bg-white
                p-4
                rounded-lg
                hover:shadow-lg hover:shadow-blue-600
              "
            >
              <div class="flex justify-between border-b items-bottom">
                <h4>{{ step.tanggal }}</h4>
                <p>{{ step.tahun }}</p>
              </div>
              <p class="mt-4 text-sm font-semibold">
                {{ step.konten }}
              </p>
            </div>
          </div>
        </div>
        <div id="section1" class="justify-between lg:flex lg:space-x-10 pr-6 pl-2">
          <div class="sm:w-3/5">
            <p class="mb-12 text-justify">
              Dalam rangka memperkuat posisi Perseroan di industri pembiayaan
              nasional, maka pada 27 Agustus 1990 Perseroan resmi melakukan
              penawaran saham perdana di Bursa Efek Jakarta (BEJ) yang kini
              bernama Bursa Efek Indonesia (BEI). Atas aksi korporasi tersebut,
              Perseroan tercatat sebagai perusahaan pembiayaan pertama yang go
              public di Indonesia.<br /><br />

              Seiring perubahan status Perseroan menjadi perusahaan terbuka,
              Perseroan kembali berganti nama menjadi PT Clipan Finance
              Indonesia Tbk, melalui keputusan Rapat Umum Pemegang Saham Luar
              Biasa No. 147 tanggal 30 Agustus 1996 juncto Akta Perubahan
              Terhadap Keputusan Rapat Umum Pemegang Saham Luar Biasa No. 190
              tanggal 23 Januari 1997 yang mana kedua akta tersebut dibuat di
              hadapan Singgih Susilo, SH, Notaris di Jakarta.<br /><br />
            </p>
          </div>
          <div class="sm:w-2/5">
            <img
              src="/background-slider.jpg"
              class="mb-8 w-full rounded-2xl"
              alt=""
            />
          </div>
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
