<template>
  <div>
    <!-- breadchum -->
    <section class="p-2">
      <div
        class="
          p-2
          bg-blue-600
          rounded-lg
          h-48
          sm:h-[320px]
          bg-[url('/background-slider.jpg')] bg-cover bg-no-repeat bg-center
        "
      >
        <div class="flex items-center mx-auto max-w-screen-xl">
          <div class="sm:w-1/2 pt-16 px-6 sm:pt-0">
            <div class="flex text-white">
              <a
                rel="noopener noreferrer"
                href="#"
                title="Back to homepage"
                class="hover:underline"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  viewBox="0 0 20 20"
                  fill="currentColor"
                  class="w-5 h-5 pr-1 dark:text-gray-400"
                >
                  <path
                    d="M10.707 2.293a1 1 0 00-1.414 0l-7 7a1 1 0 001.414 1.414L4 10.414V17a1 1 0 001 1h2a1 1 0 001-1v-2a1 1 0 011-1h2a1 1 0 011 1v2a1 1 0 001 1h2a1 1 0 001-1v-6.586l.293.293a1 1 0 001.414-1.414l-7-7z"
                  />
                </svg>
              </a>
              /
              <a
                rel="noopener noreferrer"
                href="#"
                class="flex items-center px-1 capitalize hover:underline ml-2"
                >Profile</a
              >
              /
            </div>
            <h3 class="text-black text-yellow-400">Profile Perusahaan</h3>
          </div>
          <div class="sm:w-1/2">
            <img
              src="/slider-1.png"
              loading="lazy"
              class="hidden sm:flex h-[320px] mx-auto"
            />
          </div>
        </div>
      </div>
    </section>
    <!-- menu -->
    <section class="flex w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
      <div class="flex sm:mx-auto py-4">
        <button class="btn-w ml-2 text-center sm:w-max mx-auto">
          Selengkapnya
        </button>
        <button class="btn-w ml-2 text-center sm:w-max mx-auto">
          Selengkapnya
        </button>
        <button class="btn-w ml-2 text-center sm:w-max mx-auto">
          Selengkapnya
        </button>
        <button class="btn-w ml-2 text-center sm:w-max mx-auto">
          Selengkapnya
        </button>
      </div>
    </section>

    <!-- sejarah -->
    <section class="relative py-12 dark:bg-jacarta-800">
      <div class="max-w-screen-lg mx-auto pl-4">
        <div class="sm:text-center text-left">
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
          <h3 class="hed3">Perusahaan Clipan</h3>
          <garis />
        </div>
        <p class="text-justify pr-4">
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
          <div class="flex space-x-4 ">
            <div
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
                <h3>15 Jan</h3>
                <p>1990</p>
              </div>
              <p class="mt-4">
                Berdiri dengan nama PT Clipan Leasing Corporation
              </p>
            </div>
           <div
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
                <h3>15 Jan</h3>
                <p>1990</p>
              </div>
              <p class="mt-4">
                Perubahan nama menjadi PT Clipan Finance Indonesia
              </p>
            </div>
             <div
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
                <h3>15 Jan</h3>
                <p>1990</p>
              </div>
              <p class="mt-4">
               Resmi melakukan penawaran saham perdana di BEJ
              </p>
            </div>
             <div
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
                <h4>15 Jan</h4>
                <p>1990</p>
              </div>
              <p class="mt-4">
               Berganti nama menjadi PT Clipan Finance Indonesia Tbk
              </p>
            </div>
          </div>
        </div>
        <div class="justify-between lg:flex lg:space-x-10 pr-4">
          <div class="sm:w-3/5">
            <p class="mb-12">
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
  </div>
</template>
