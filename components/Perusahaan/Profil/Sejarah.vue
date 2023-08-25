<template>
  <section class="relative sm:mt-24 py-12 dark:bg-jacarta-800">
    <div class="max-w-screen-lg mx-auto pl-4">
      <div
        id="section1"
        class="justify-between lg:flex lg:space-x-10 pr-6 pl-2"
      >

        <div class="sm:w-2/5 p-4 sm:p-0">
          <div class="relative">
            <div
              class="
                absolute
                h-full
                w-full
                grid grid-cols-3
                place-content-between
                animate-fly
              "
            >
              <div>
                <div
                  class="
                    text-center
                    bg-blue-600
                    rounded-lg
                    shadow-lg
                    w-max
                    p-5
                    text-white
                    scale-95
                    hover:scale-100
                    duration-200
                  "
                >
                  <p class="text-sm -mb-3">Lebih dari</p>
                  <h3 class="text-4xl text-white -mt-2">40</h3>
                  <p class="text-sm -mt-3">Berdiri</p>
                </div>
              </div>
              <div></div>
              <div>
                <div
                  class="
                    text-center
                    bg-gray-50
                    rounded-lg
                    shadow-lg
                    w-max
                    p-5
                    text-blue-600
                    mt-12
                    scale-95
                    hover:scale-100
                    duration-200
                  "
                >
                  <h3 class="text-4xl text-blue-600 -mt-2">+7</h3>
                  <p class="text-sm -mt-3">Triliun Aset</p>
                </div>
              </div>
              <div class="col-span-3"></div>
              <div
                class="
                  text-center
                  bg-blue-600
                  rounded-lg
                  shadow-lg
                  w-max
                  p-5
                  ml-4
                  mt-14
                  text-white
                  scale-95
                  hover:scale-100
                  duration-200
                "
              >
                <h3 class="text-4xl text-white -mt-2">3000</h3>
                <p class="text-sm -mt-3">lebih Karyawan</p>
              </div>

              <div></div>
              <div
                class="
                  text-center
                  bg-blue-600
                  rounded-lg
                  shadow-lg
                  w-max
                  p-5
                  mb-10
                  ml-10
                  text-white
                  scale-95
                  hover:scale-100
                  duration-200
                "
              >
                <p class="text-sm -mb-3">Memiliki</p>
                <h3 class="text-4xl text-white -mt-2">63</h3>
                <p class="text-sm -mt-3">Cabang</p>
              </div>
            </div>

            <img
              src="/wisma-slipi.png"
              class="mb-8 w-full rounded-2xl"
              alt=""
            />
          </div>
        </div>
                <div class="sm:w-3/5">
          <div class="text-left ">
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
              >Sejarah Singkat</span
            >
            <h1 class="hed3 mt-2">Clipan Finance Indonesia</h1>
            <garis />

        <h3 class="hed4 pb-5 ">
         Clipan Finance adalah bagian dari Panin Group, perusahaan dengan
            pengalaman sejak 1982 di industri pembiayaan. 
        </h3>
          </div>
          <p class="text-justify">
           Fokus utama kami
            adalah memberikan pembiayaan untuk mobil baru, mobil bekas, alat
            berat, dan multiguna. Visi kami adalah menjadi perusahaan pembiayaan
            terkemuka yang membantu masyarakat Indonesia mencapai impian mereka.
            Kami menawarkan pelayanan terbaik dan solusi finansial yang tepat
            sesuai kebutuhan pelanggan.
            <br /><br />
            PT Clipan Finance Indonesia Tbk (“Perseroan”) pertama kali didirikan
            dengan nama PT Clipan Leasing Corporation berdasarkan Akta No. 47
            pada 15 Januari 1982 yang dibuat dihadapan Kartini Muljadi, S.H.,
            Notaris di Jakarta. Dalam tonggak sejarah berikutnya, tepatnya pada
            17 Mei 1990, Perseroan melakukan perubahan nama dari semula PT
            Clipan Leasing Corporation menjadi PT Clipan Finance Indonesia yang
            mana perubahan tersebut mengacu pada Akta No. 56 tanggal 17 Mei 1990
            dan telah disahkan melalui Surat Keputusan Menteri Kehakiman
            Republik Indonesia No. C2.3418.HT.01.04.th 90 tanggal 5 Juli 1990.
          </p>
        </div>
      </div>
      <div
        class="flex py-12 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto"
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
      <div>
        <p class="mb-12 text-justify pr-4">
          Dalam rangka memperkuat posisi Perseroan di industri pembiayaan
          nasional, maka pada 27 Agustus 1990 Perseroan resmi melakukan
          penawaran saham perdana di Bursa Efek Jakarta (BEJ) yang kini bernama
          Bursa Efek Indonesia (BEI). Atas aksi korporasi tersebut, Perseroan
          tercatat sebagai perusahaan pembiayaan pertama yang go public di
          Indonesia.<br /><br />

          Seiring perubahan status Perseroan menjadi perusahaan terbuka,
          Perseroan kembali berganti nama menjadi PT Clipan Finance Indonesia
          Tbk, melalui keputusan Rapat Umum Pemegang Saham Luar Biasa No. 147
          tanggal 30 Agustus 1996 juncto Akta Perubahan Terhadap Keputusan Rapat
          Umum Pemegang Saham Luar Biasa No. 190 tanggal 23 Januari 1997 yang
          mana kedua akta tersebut dibuat di hadapan Singgih Susilo, SH, Notaris
          di Jakarta.<br /><br />
        </p>
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
