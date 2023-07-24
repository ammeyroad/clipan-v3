<template>
  <div class="p-2">
    <div
      class="
        group
        relative
        flex
        h-72
        sm:h-[400px]
        items-center
        px-12
        overflow-hidden
        rounded-lg
        bg-gray-100 bg-gradient-to-tr
        from-blue-400
        to-blue-600
      "
    >
      <img
        src="https://images.unsplash.com/photo-1618556450991-2f1af64e8191?auto=format&q=75&fit=crop&w=1000"
        loading="lazy"
        class="
          absolute
          inset-0
          h-full
          w-full
          object-cover object-center
          opacity-25
          transition
          duration-200
        "
      />
      <div class="relative text-white mt-24">
        <ol class="flex h-8 space-x-2">
          <li class="flex items-center">
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
          </li>
          <li class="flex items-center space-x-2">
            /
            <a
              rel="noopener noreferrer"
              href="#"
              class="flex items-center px-1 capitalize hover:underline ml-2"
              >Profile</a
            >
          </li>
          <li class="flex items-center space-x-2">/</li>
        </ol>
        <h3 class="text-black-800 text-xl font-bold md:text-2xl">
          Tata Kelola Perusahaan
        </h3>
      </div>
    </div>
  </div>
  <ul
    class="
      w-full
      md:mx-auto md:max-w-screen-xl
      flex
      justify-between
      items-start
      mb-8
      space-x-3
      overflow-x-auto
      p-2
    "
  >
    <li class="flex w-full mx-auto">
      <button
        type="button"
        class="
          w-max
          py-2.5
          bg-white
          px-5
          mr-2
          mb-2
          text-sm
          font-medium
          text-gray-900
          focus:outline-none
          rounded-lg
          hover:bg-blue-600 hover:text-white
          focus:z-10 focus:ring-4 focus:ring-gray-200
        "
      >
        Alternative
      </button>
    </li>
  </ul>

  <!-- sejarah singkat -->
  <section class="max-w-screen-lg px-5 mx-auto space-y-12">
    <div class="">
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
      <h3 class="text-blue-600 text-2xl pt-2 font-bold md:text-4xl">
        Perusahaan Clipan
      </h3>
      <garis />
    </div>

    <div class="grid sm:grid-cols-5 sm:space-x-16">
      <div class="sm:col-span-2">
        <img
          src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
          loading="lazy"
          alt="Photo by Fakurian Design"
          class=""
        />
      </div>
      <div class="sm:col-span-3">
        <p class="text-left">
          Berawal dari marketplace lalu tumbuh menjadi platform yang memberikan
          banyak kemudahan untuk berbisnis. Inilah kami, Buka, perusahaan yang
          terus berevolusi dan berinovasi untuk kepentingan bersama.
          <br /><br />

          Dalam tonggak sejarah berikutnya, tepatnya pada 17 Mei 1990, Perseroan
          melakukan perubahan nama dari semula PT Clipan Leasing Corporation
          menjadi PT Clipan Finance Indonesia yang mana perubahan tersebut
          mengacu pada Akta No. 56 tanggal 17 Mei 1990 dan telah disahkan
          melalui Surat Keputusan Menteri Kehakiman Republik Indonesia No.
          C2.3418.HT.01.04.th 90 tanggal 5 Juli 1990.
          <br /><br />

          Dalam rangka memperkuat posisi Perseroan di industri pembiayaan
          nasional, maka pada 27 Agustus 1990 Perseroan resmi melakukan
          penawaran saham perdana di Bursa Efek Jakarta (BEJ) yang kini bernama
          Bursa Efek Indonesia (BEI). Atas aksi korporasi tersebut, Perseroan
          tercatat sebagai perusahaan pembiayaan pertama yang go public di
          Indonesia.
        </p>
      </div>
    </div>

    <div class="flex w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
      <div class="flex space-x-4">
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
      </div>
    </div>
  </section>

  <!-- visimisi dan budaya -->
  <section class="bg-white px-5 mt-24 py-12">
    <div class="max-w-screen-lg mx-auto space-y-12">
      <div class="text-left">
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
          >Mengenal Lebih</span
        >
        <h3 class="text-blue-600 text-2xl pt-2 font-bold md:text-4xl">
          VISI, Misi dan Budaya
        </h3>
        <garis />
      </div>

      <div class="kungar flex p-5 rounded-lg space-x-10">
        <div class="w-2/5">
          <div class="head2 mb-2">VISI</div>
          <p>
            Menjadi perusahaan pembiayaan terkemuka yang mengedepankan nilai
            tambah bagi pemangku kepentingan dan berperan aktif dalam
            pertumbuhan industri pembiayaan nasional.
          </p>
        </div>

        <div>
          <div class="head2 mb-2">Misi</div>

          <ul class="list-outside list-disc ... ml-4">
            <li>
              Menyediakan produk dan jasa keuangan yang inovatif didukung sumber
              daya manusia yang handal dan teknologi terkini.
            </li>
            <li>
              Mempertahankan dan meningkatkan kinerja keuangan yang sehat dan
              berkelanjutan.
            </li>
            <li>
              Menjalankan perusahaan sesuai dengan prinsip-prinsip tata kelola
              perusahaan yang baik.
            </li>
          </ul>
        </div>
      </div>
      <div>
        <div>
          <div class="head3">Budaya Perusahaan</div>
          <p>
            Menyediakan produk dan jasa keuangan yang inovatif didukung sumber
            daya manusia yang handal dan teknologi terkini.
          </p>
        </div>

        <!-- <div class="flex mt-5 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
        <div class="flex space-x-4">
         <div class="w-52 sm:w-1/5 bg-blue-400 p-4">
           <div class="flex items-center">
            <div
              class="
                flex
                h-12
                w-12
                shrink-0
                items-center
                justify-center
                rounded-lg
                bg-indigo-500
                text-white
                shadow-lg
                md:h-14 md:w-14 md:rounded-xl
              "
            >
              <p class="head4">C</p>
            </div>
           <p class="ml-2 font-bold uppercase">reative</p>
           </div>
            <p class="mt-4">
              Menyediakan produk dan jasa keuangan yang inovatif didukung sumber
              daya manusia yang handal dan teknologi terkini.
            </p>
          </div>
            <div class="w-52 sm:w-1/5 bg-blue-400 p-4">
           <div class="flex items-center">
            <div
              class="
                flex
                h-12
                w-12
                shrink-0
                items-center
                justify-center
                rounded-lg
                bg-indigo-500
                text-white
                shadow-lg
                md:h-14 md:w-14 md:rounded-xl
              "
            >
              <p class="head4">C</p>
            </div>
           <p class="ml-2 font-bold uppercase">reative</p>
           </div>
            <p class="mt-4">
              Menyediakan produk dan jasa keuangan yang inovatif didukung sumber
              daya manusia yang handal dan teknologi terkini.
            </p>
          </div>
            <div class="w-52 sm:w-1/5 bg-blue-400 p-4">
           <div class="flex items-center">
            <div
              class="
                flex
                h-12
                w-12
                shrink-0
                items-center
                justify-center
                rounded-lg
                bg-indigo-500
                text-white
                shadow-lg
                md:h-14 md:w-14 md:rounded-xl
              "
            >
              <p class="head4">C</p>
            </div>
           <p class="ml-2 font-bold uppercase">reative</p>
           </div>
            <p class="mt-4">
              Menyediakan produk dan jasa keuangan yang inovatif didukung sumber
              daya manusia yang handal dan teknologi terkini.
            </p>
          </div>
            <div class="w-52 sm:w-1/5 bg-blue-400 p-4">
           <div class="flex items-center">
            <div
              class="
                flex
                h-12
                w-12
                shrink-0
                items-center
                justify-center
                rounded-lg
                bg-indigo-500
                text-white
                shadow-lg
                md:h-14 md:w-14 md:rounded-xl
              "
            >
              <p class="head4">C</p>
            </div>
           <p class="ml-2 font-bold uppercase">reative</p>
           </div>
            <p class="mt-4">
              Menyediakan produk dan jasa keuangan yang inovatif didukung sumber
              daya manusia yang handal dan teknologi terkini.
            </p>
          </div>
            <div class="w-52 sm:w-1/5 bg-blue-400 p-4">
           <div class="flex items-center">
            <div
              class="
                flex
                h-12
                w-12
                shrink-0
                items-center
                justify-center
                rounded-lg
                bg-indigo-500
                text-white
                shadow-lg
                md:h-14 md:w-14 md:rounded-xl
              "
            >
              <p class="head4">C</p>
            </div>
           <p class="ml-2 font-bold uppercase">reative</p>
           </div>
            <p class="mt-4">
              Menyediakan produk dan jasa keuangan yang inovatif didukung sumber
              daya manusia yang handal dan teknologi terkini.
            </p>
          </div>
        </div>
      </div> -->
      </div>
    </div>
  </section>
  <div class="flex mt-5 w-full overflow-x-auto">
    <div class="flex py-12">
      <div
      
        class="
          w-72
          ml-8
          snap-center
          block
          rounded-2xl
          border border-jacarta-100
          bg-white
          p-2
          text-gray-600
          hover:text-blue-600
          transition-shadow
          hover:shadow-lg
        "
      >
        <figure class="relative">
          <a href="item.html">
            <img
              src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
              alt="item 5"
              class="h-64 rounded-[0.625rem]"
              loading="lazy"
            />
          </a>
          <div
            class="
              absolute
              top-3
              right-3
              flex
              items-center
              space-x-1
              rounded-md
              bg-white
              p-2
            "
          >
            <span class="text-sm dark:text-jacarta-200">Mobil Baru</span>
          </div>
          <div class="absolute right-3 -bottom-5">
            <div class="flex">
              <a href="#">
                <img
                  src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
                  alt="owner"
                  class="
                    h-10
                    w-10
                    rounded-full
                    border-2 border-white
                    hover:border-accent
                    dark:border-jacarta-600 dark:hover:border-accent
                  "
                  data-tippy-content="Owner: Sussygirl"
                />
              </a>
            </div>
          </div>
        </figure>
        <div class="p-2">
          <div class="mt-4 flex items-center justify-between">
            <a href="item.html">
              <span class="font-bold "
                >Mitsubishi <br />
                PAJERO SPORT DAKAR 4X2 2.4</span
              >
            </a>
          </div>
          <div class="mt-2 flex space-x-1 w-full overflow-x-auto text-xs text-gray-900">
            <div
              class="
                flex
                items-center
                bg-gray-100
                w-max
                p-2
                rounded
                opacity-50
                hover:opacity-100 hover:fill-blue-600 hover:text-blue-600
              "
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                class="w-4"
              >
                <path
                  d="M12 19a1 1 0 1 0-1-1a1 1 0 0 0 1 1Zm5 0a1 1 0 1 0-1-1a1 1 0 0 0 1 1Zm0-4a1 1 0 1 0-1-1a1 1 0 0 0 1 1Zm-5 0a1 1 0 1 0-1-1a1 1 0 0 0 1 1Zm7-12h-1V2a1 1 0 0 0-2 0v1H8V2a1 1 0 0 0-2 0v1H5a3 3 0 0 0-3 3v14a3 3 0 0 0 3 3h14a3 3 0 0 0 3-3V6a3 3 0 0 0-3-3Zm1 17a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1v-9h16Zm0-11H4V6a1 1 0 0 1 1-1h1v1a1 1 0 0 0 2 0V5h8v1a1 1 0 0 0 2 0V5h1a1 1 0 0 1 1 1ZM7 15a1 1 0 1 0-1-1a1 1 0 0 0 1 1Zm0 4a1 1 0 1 0-1-1a1 1 0 0 0 1 1Z"
                />
              </svg>
              <span class="ml-1">2012</span>
            </div>
            <div
              class="
                flex
                items-center
                bg-gray-100
                w-max
                p-2
                rounded
                opacity-50
                hover:opacity-100 hover:fill-blue-600 hover:text-blue-600
              "
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="w-4"
                viewBox="0 0 24 24"
              >
                <path
                  fill="#888888"
                  d="M12 11a1 1 0 1 0 1 1a1 1 0 0 0-1-1Zm0-9a10 10 0 1 0 10 10A10 10 0 0 0 12 2Zm1 17.93V17a1 1 0 0 0-2 0v2.93A8 8 0 0 1 4.07 13H7a1 1 0 0 0 0-2H4.07A8 8 0 0 1 11 4.07V7a1 1 0 0 0 2 0V4.07A8 8 0 0 1 19.93 11H17a1 1 0 0 0 0 2h2.93A8 8 0 0 1 13 19.93Z"
                />
              </svg>
              <span class="ml-1">Matic</span>
            </div>
            <div
              class="
                flex
                items-center
                bg-gray-100
                w-max
                p-2
                rounded
                opacity-50
                hover:opacity-100 hover:fill-blue-600 hover:text-blue-600
              "
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="w-4"
                viewBox="0 0 24 24"
              >
                <path
                  fill="#888888"
                  d="M11 11.9V17a1 1 0 0 0 2 0v-5.1a5 5 0 1 0-2 0ZM12 4a3 3 0 1 1-3 3a3 3 0 0 1 3-3Zm4.21 10.42a1 1 0 1 0-.42 2C18.06 16.87 19 17.68 19 18c0 .58-2.45 2-7 2s-7-1.42-7-2c0-.32.94-1.13 3.21-1.62a1 1 0 1 0-.42-2C4.75 15.08 3 16.39 3 18c0 2.63 4.53 4 9 4s9-1.37 9-4c0-1.61-1.75-2.92-4.79-3.58Z"
                />
              </svg>
              <span class="ml-1"> 12.123 km</span>
            </div>
          </div>

          <div class="mt-8 flex items-bottom justify-between">
            <p>
              <sub>Mulai dari </sub><br />
              <span class="text-lg font-bold text-blue-600">Rp. 20.000.000</span>
              <span class="text-xs"> /bulan</span>
            </p>
            <p>
             <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" class="mt-6" viewBox="0 0 24 24"><path fill="#888888" d="M20.16 5A6.29 6.29 0 0 0 12 4.36a6.27 6.27 0 0 0-8.16 9.48l6.21 6.22a2.78 2.78 0 0 0 3.9 0l6.21-6.22a6.27 6.27 0 0 0 0-8.84Zm-1.41 7.46l-6.21 6.21a.76.76 0 0 1-1.08 0l-6.21-6.24a4.29 4.29 0 0 1 0-6a4.27 4.27 0 0 1 6 0a1 1 0 0 0 1.42 0a4.27 4.27 0 0 1 6 0a4.29 4.29 0 0 1 .08 6Z"/></svg>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
useHead({
  title: 'aksii',
  titleTemplate: '%s - Clipan Finance Indonesia',
  meta: [{ name: 'description', content: 'Clipan Finance Indonesia' }],
});
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@400;500;800&family=Nunito:ital,wght@0,500;0,900;0,1000;1,900&display=swap');
</style>
