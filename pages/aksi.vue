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
      <div class="flex mt-5 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
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
      </div>
      </div>
      <div class="grid sm:gap-20">
        <div class=""></div>
        <div class="">
          <div class="grid gap-8 sm:grid-cols-5">
            <!-- feature - start -->
            <div class="flex gap-4 md:gap-6">
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
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"
                  />
                </svg>
              </div>

              <div>
                <h3 class="mb-2 text-lg font-semibold md:text-xl">Growth</h3>
                <p class="mb-2 text-gray-500">
                  Filler text is dummy text which has no meaning however looks
                  very similar to real text.
                </p>
                <a
                  href="#"
                  class="
                    font-bold
                    text-indigo-500
                    transition
                    duration-100
                    hover:text-indigo-600
                    active:text-indigo-700
                  "
                  >More</a
                >
              </div>
            </div>
            <!-- feature - end -->

            <!-- feature - start -->
            <div class="flex gap-4 md:gap-6">
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
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"
                  />
                </svg>
              </div>

              <div>
                <h3 class="mb-2 text-lg font-semibold md:text-xl">Security</h3>
                <p class="mb-2 text-gray-500">
                  Filler text is dummy text which has no meaning however looks
                  very similar to real text.
                </p>
                <a
                  href="#"
                  class="
                    font-bold
                    text-indigo-500
                    transition
                    duration-100
                    hover:text-indigo-600
                    active:text-indigo-700
                  "
                  >More</a
                >
              </div>
            </div>
            <!-- feature - end -->

            <!-- feature - start -->
            <div class="flex gap-4 md:gap-6">
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
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M3 15a4 4 0 004 4h9a5 5 0 10-.1-9.999 5.002 5.002 0 10-9.78 2.096A4.001 4.001 0 003 15z"
                  />
                </svg>
              </div>

              <div>
                <h3 class="mb-2 text-lg font-semibold md:text-xl">Cloud</h3>
                <p class="mb-2 text-gray-500">
                  Filler text is dummy text which has no meaning however looks
                  very similar to real text.
                </p>
                <a
                  href="#"
                  class="
                    font-bold
                    text-indigo-500
                    transition
                    duration-100
                    hover:text-indigo-600
                    active:text-indigo-700
                  "
                  >More</a
                >
              </div>
            </div>
            <!-- feature - end -->

            <!-- feature - start -->
            <div class="flex gap-4 md:gap-6">
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
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M13 10V3L4 14h7v7l9-11h-7z"
                  />
                </svg>
              </div>

              <div>
                <h3 class="mb-2 text-lg font-semibold md:text-xl">Speed</h3>
                <p class="mb-2 text-gray-500">
                  Filler text is dummy text which has no meaning however looks
                  very similar to real text.
                </p>
                <a
                  href="#"
                  class="
                    font-bold
                    text-indigo-500
                    transition
                    duration-100
                    hover:text-indigo-600
                    active:text-indigo-700
                  "
                  >More</a
                >
              </div>
            </div>
            <!-- feature - end -->

            <!-- feature - start -->
            <div class="flex gap-4 md:gap-6">
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
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M18.364 5.636l-3.536 3.536m0 5.656l3.536 3.536M9.172 9.172L5.636 5.636m3.536 9.192l-3.536 3.536M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-5 0a4 4 0 11-8 0 4 4 0 018 0z"
                  />
                </svg>
              </div>

              <div>
                <h3 class="mb-2 text-lg font-semibold md:text-xl">Support</h3>
                <p class="mb-2 text-gray-500">
                  Filler text is dummy text which has no meaning however looks
                  very similar to real text.
                </p>
                <a
                  href="#"
                  class="
                    font-bold
                    text-indigo-500
                    transition
                    duration-100
                    hover:text-indigo-600
                    active:text-indigo-700
                  "
                  >More</a
                >
              </div>
            </div>
            <!-- feature - end -->

            <!-- feature - start -->
            <div class="flex gap-4 md:gap-6">
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
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"
                  />
                </svg>
              </div>

              <div>
                <h3 class="mb-2 text-lg font-semibold md:text-xl">Dark Mode</h3>
                <p class="mb-2 text-gray-500">
                  Filler text is dummy text which has no meaning however looks
                  very similar to real text.
                </p>
                <a
                  href="#"
                  class="
                    font-bold
                    text-indigo-500
                    transition
                    duration-100
                    hover:text-indigo-600
                    active:text-indigo-700
                  "
                  >More</a
                >
              </div>
            </div>
            <!-- feature - end -->
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup>
useHead({
  title: 'aksii',
  titleTemplate: '%s - Clipan Finance Indonesia',
  meta: [{ name: 'description', content: 'Clipan Finance Indonesia' }],
});
</script>
