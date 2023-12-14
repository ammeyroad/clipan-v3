<template>
  <section class=" py-24">
    <div class="max-w-screen-lg px-5 mx-auto space-y-12">
      <div class="grid grid-cols-1 sm:gap-10 sm:grid-cols-12">
        <!-- simulasi -->
        <div class="col-span-7 mb-10">
          <div class="text-left mb-10">
            <p class="font-semibold text-sm xl:text-xl"></p>
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
              >Skema Perhitungan</span
            >
            <h3 class=" text-2xl pt-2 font-bold md:text-4xl">
              Simulasi Mobil Baru
            </h3>
            <garis />

           
          </div>
          <SimulasiNew />
        </div>
        <!-- hasil simulasi -->
        <div
          class="
            col-span-5
            relative
            rounded-xl
            border
            p-2
            bg-white
            overflow-hidden
            shadow-[0_5px_0_0_#10b981]
            transition-shadow
            hover:shadow-[0_16px_24px_-8px_rgba(16,185,129,.3)]
          "
        >
          <!-- <div class="text-center mb-6">
        <p class="font-bold text-lg text-yellow-500">Skema</p>
        <h3 class="mb-4 font-bold text-xl">Perhitungan</h3>
        <p class="">
          Detail bunga dalam pembiayaan dengan jamina n BPKB mobil :
        </p>
      </div> -->

          <!-- <div v-for="n in 4" class="flex border-b py-2 justify-between">
        <p>bunga perBulan</p>
        <p>0,8%</p>
      </div> -->

          <SimulasiHasil />
        </div>
      </div>
    </div>
  </section>

  <section class="grid h-max content-center bg-blue-600/5">
    <div class="container mx-auto mt-12 items-center gap-12 p-6 sm:my-16">
      <div class="text-center text-gray-700">
        <div>
          <span
            class="
              rounded-full
              bg-yellow-400
              px-2.5
              py-1.5
              text-center text-xs
              font-bold
              uppercase
            "
            >Penjelasan Mobil Baru</span
          >
          <h1
            class="
              my-2
              mb-6
              text-2xl
              font-bold
              capitalize
              text-blue-600
              drop-shadow
            "
          >
            Heading promo mobil baru disini
          </h1>
          <p class="mx-auto mb-8 max-w-screen-md leading-relaxed">
            Clipan Finance merupakan anak perusahaan Bank Panin yang menyediakan
            fasilitas pembiayaan mobil baru dengan beragam program pembiayaan
            yang menarik.
          </p>
          <div class="flex justify-center gap-2">
            <a
              href="#"
              class="
                mb-2
                me-2
                rounded-full
                border border-blue-600
                bg-blue-600
                px-5
                py-2.5
                text-sm
                font-bold
                uppercase
                text-white
                hover:bg-blue-700
                hover:text-yellow-400
                hover:shadow-lg
                hover:shadow-blue-700/50
                focus:z-10 focus:outline-none focus:ring-4 focus:ring-gray-200
              "
              >KPM Panin</a
            >
            <a
              href="#"
              class="
                mb-2
                me-2
                rounded-full
                border border-blue-600
                bg-transparent
                px-5
                py-2.5
                text-sm
                font-bold
                uppercase
                text-blue-600
                hover:bg-blue-700
                hover:text-yellow-400
                hover:shadow-lg
                hover:shadow-blue-700/50
                focus:z-10 focus:outline-none focus:ring-4 focus:ring-gray-200
              "
              >Syarat Kredit</a
            >
          </div>
        </div>
        <div
          class="
            mx-auto
            mt-16
            grid
            max-w-screen-lg
            grid-cols-2
            divide-x divide-y divide-gray-100
            overflow-hidden
            rounded-xl
            border
            shadow-xl
            hover:border-0
            sm:grid-cols-4
            lg:divide-y-0
            xl:grid-cols-4
          "
        >
          <div
            class="
              group
              bg-white
              transition
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-xl
              hover:shadow-blue-600/10
            "
          >
            <div class="space-y-8 p-4 py-8">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mx-auto h-10 w-10"
              >
                <path
                  fill-rule="evenodd"
                  d="M17.303 5.197A7.5 7.5 0 006.697 15.803a.75.75 0 01-1.061 1.061A9 9 0 1121 10.5a.75.75 0 01-1.5 0c0-1.92-.732-3.839-2.197-5.303zm-2.121 2.121a4.5 4.5 0 00-6.364 6.364.75.75 0 11-1.06 1.06A6 6 0 1118 10.5a.75.75 0 01-1.5 0c0-1.153-.44-2.303-1.318-3.182zm-3.634 1.314a.75.75 0 01.82.311l5.228 7.917a.75.75 0 01-.777 1.148l-2.097-.43 1.045 3.9a.75.75 0 01-1.45.388l-1.044-3.899-1.601 1.42a.75.75 0 01-1.247-.606l.569-9.47a.75.75 0 01.554-.68z"
                  clip-rule="evenodd"
                />
              </svg>

              <div class="space-y-2">
                <h5
                  class="
                    text-xl
                    font-medium
                    text-blue-600
                    group-hover:text-yellow-400
                  "
                >
                  First feature
                </h5>
                <p class="text-sm">
                  Neque Dolor, fugiat non cum doloribus aperiam voluptates
                  nostrum.
                </p>
              </div>
            </div>
          </div>
          <div
            class="
              group
              bg-white
              transition
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-xl
              hover:shadow-blue-600/10
            "
          >
            <div class="space-y-8 p-4 py-8">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mx-auto h-10 w-10"
              >
                <path
                  fill-rule="evenodd"
                  d="M17.303 5.197A7.5 7.5 0 006.697 15.803a.75.75 0 01-1.061 1.061A9 9 0 1121 10.5a.75.75 0 01-1.5 0c0-1.92-.732-3.839-2.197-5.303zm-2.121 2.121a4.5 4.5 0 00-6.364 6.364.75.75 0 11-1.06 1.06A6 6 0 1118 10.5a.75.75 0 01-1.5 0c0-1.153-.44-2.303-1.318-3.182zm-3.634 1.314a.75.75 0 01.82.311l5.228 7.917a.75.75 0 01-.777 1.148l-2.097-.43 1.045 3.9a.75.75 0 01-1.45.388l-1.044-3.899-1.601 1.42a.75.75 0 01-1.247-.606l.569-9.47a.75.75 0 01.554-.68z"
                  clip-rule="evenodd"
                />
              </svg>

              <div class="space-y-2">
                <h5
                  class="
                    text-xl
                    font-medium
                    text-blue-600
                    group-hover:text-yellow-400
                  "
                >
                  First feature
                </h5>
                <p class="text-sm">
                  Neque Dolor, fugiat non cum doloribus aperiam voluptates
                  nostrum.
                </p>
              </div>
            </div>
          </div>
          <div
            class="
              group
              bg-white
              transition
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-xl
              hover:shadow-blue-600/10
            "
          >
            <div class="space-y-8 p-4 py-8">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mx-auto h-10 w-10"
              >
                <path
                  fill-rule="evenodd"
                  d="M17.303 5.197A7.5 7.5 0 006.697 15.803a.75.75 0 01-1.061 1.061A9 9 0 1121 10.5a.75.75 0 01-1.5 0c0-1.92-.732-3.839-2.197-5.303zm-2.121 2.121a4.5 4.5 0 00-6.364 6.364.75.75 0 11-1.06 1.06A6 6 0 1118 10.5a.75.75 0 01-1.5 0c0-1.153-.44-2.303-1.318-3.182zm-3.634 1.314a.75.75 0 01.82.311l5.228 7.917a.75.75 0 01-.777 1.148l-2.097-.43 1.045 3.9a.75.75 0 01-1.45.388l-1.044-3.899-1.601 1.42a.75.75 0 01-1.247-.606l.569-9.47a.75.75 0 01.554-.68z"
                  clip-rule="evenodd"
                />
              </svg>

              <div class="space-y-2">
                <h5
                  class="
                    text-xl
                    font-medium
                    text-blue-600
                    group-hover:text-yellow-400
                  "
                >
                  First feature
                </h5>
                <p class="text-sm">
                  Neque Dolor, fugiat non cum doloribus aperiam voluptates
                  nostrum.
                </p>
              </div>
            </div>
          </div>
          <div
            class="
              group
              bg-white
              transition
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-xl
              hover:shadow-blue-600/10
            "
          >
            <div class="space-y-8 p-4 py-8">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="mx-auto h-10 w-10"
              >
                <path
                  fill-rule="evenodd"
                  d="M17.303 5.197A7.5 7.5 0 006.697 15.803a.75.75 0 01-1.061 1.061A9 9 0 1121 10.5a.75.75 0 01-1.5 0c0-1.92-.732-3.839-2.197-5.303zm-2.121 2.121a4.5 4.5 0 00-6.364 6.364.75.75 0 11-1.06 1.06A6 6 0 1118 10.5a.75.75 0 01-1.5 0c0-1.153-.44-2.303-1.318-3.182zm-3.634 1.314a.75.75 0 01.82.311l5.228 7.917a.75.75 0 01-.777 1.148l-2.097-.43 1.045 3.9a.75.75 0 01-1.45.388l-1.044-3.899-1.601 1.42a.75.75 0 01-1.247-.606l.569-9.47a.75.75 0 01.554-.68z"
                  clip-rule="evenodd"
                />
              </svg>

              <div class="space-y-2">
                <h5
                  class="
                    text-xl
                    font-medium
                    text-blue-600
                    group-hover:text-yellow-400
                  "
                >
                  First feature
                </h5>
                <p class="text-sm">
                  Neque Dolor, fugiat non cum doloribus aperiam voluptates
                  nostrum.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- persyaratan -->
  <section class="-mt-48 grid h-max content-center bg-blue-600 py-32">
    <div
      class="container mx-auto mt-24 items-center gap-12 p-6 sm:my-16 sm:flex"
    >
      <div class="sm:w-2/5">
        <span
          class="
            rounded-full
            bg-yellow-400
            px-2.5
            py-1.5
            text-center text-xs
            font-bold
            uppercase
          "
          >Syarat</span
        >
        <h1
          class="my-2 mb-6 text-2xl font-bold capitalize text-white drop-shadow"
        >
          Perysaratan Kredit
        </h1>
        <p class="mx-auto mb-8 max-w-screen-md leading-relaxed text-white">
          Clipan Finance merupakan anak perusahaan Bank Panin yang menyediakan
          fasilitas pembiayaan mobil baru dengan beragam program pembiayaan yang
          menarik.
        </p>
        <div
          class="
            grid grid-cols-3
            gap-1
            rounded-xl
            bg-black/10
            p-1
            sm:grid-cols-1 sm:gap-4 sm:bg-transparent
          "
        >
          <button
            type="button"
            class="
              flex
              items-center
              rounded-lg
              border border-black/10
              bg-yellow-400
              py-3
              pl-2
              text-center text-base
              font-medium
              text-black
              hover:bg-yellow-500
              focus:outline-none focus:ring-4 focus:ring-yellow-300
            "
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="currentColor"
              class="mr-2 h-4 w-4"
            >
              <path
                fill-rule="evenodd"
                d="M7.5 6a4.5 4.5 0 119 0 4.5 4.5 0 01-9 0zM3.751 20.105a8.25 8.25 0 0116.498 0 .75.75 0 01-.437.695A18.683 18.683 0 0112 22.5c-2.786 0-5.433-.608-7.812-1.7a.75.75 0 01-.437-.695z"
                clip-rule="evenodd"
              />
            </svg>
            <span class="text-xs font-semibold uppercase sm:text-lg"
              >Perorangan</span
            >
          </button>
          <button
            type="button"
            class="
              flex
              items-center
              rounded-lg
              border border-black/10
              bg-white/10
              py-3
              pl-2
              text-center text-base
              font-medium
              text-white
              hover:bg-yellow-400 hover:text-black
              focus:outline-none focus:ring-4 focus:ring-yellow-300
            "
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="currentColor"
              class="mr-2 h-4 w-4"
            >
              <path
                fill-rule="evenodd"
                d="M7.5 6a4.5 4.5 0 119 0 4.5 4.5 0 01-9 0zM3.751 20.105a8.25 8.25 0 0116.498 0 .75.75 0 01-.437.695A18.683 18.683 0 0112 22.5c-2.786 0-5.433-.608-7.812-1.7a.75.75 0 01-.437-.695z"
                clip-rule="evenodd"
              />
            </svg>
            <span class="text-xs font-semibold uppercase sm:text-lg"
              >perusahaan</span
            >
          </button>
          <button
            type="button"
            class="
              flex
              items-center
              rounded-lg
              border border-black/10
              bg-white/10
              py-3
              pl-2
              text-center text-base
              font-medium
              text-white
              hover:bg-yellow-400 hover:text-black
              focus:outline-none focus:ring-4 focus:ring-yellow-300
            "
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="currentColor"
              class="mr-2 h-4 w-4"
            >
              <path
                fill-rule="evenodd"
                d="M7.5 6a4.5 4.5 0 119 0 4.5 4.5 0 01-9 0zM3.751 20.105a8.25 8.25 0 0116.498 0 .75.75 0 01-.437.695A18.683 18.683 0 0112 22.5c-2.786 0-5.433-.608-7.812-1.7a.75.75 0 01-.437-.695z"
                clip-rule="evenodd"
              />
            </svg>
            <span class="text-xs font-semibold uppercase sm:text-lg"
              >perusahaan</span
            >
          </button>
        </div>
      </div>
      <div class="mt-6 sm:mt-0 sm:w-3/5">
        <div
          class="
            rounded-lg
            border-2 border-white
            bg-gradient-to-br
            from-white
            to-gray-50
            p-6
            shadow-xl
          "
        >
          <h1
            class="
              mb-2
              border-b
              pb-2
              text-lg
              font-semibold
              uppercase
              text-blue-600
            "
          >
            Syarat untuk Karyawan
          </h1>
          <ul
            class="
              gap-
              grid
              list-inside
              space-y-1
              text-gray-500
              dark:text-gray-400
              sm:grid-cols-2
            "
          >
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              Identitas Pemohon
            </li>
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              Identitas Penjamin*
            </li>
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              Kartu Keluarga atau akte nikah
            </li>
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              Surat Cerai/Surat Kematian**
            </li>
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              NPWP
            </li>
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              Slip Gaji
            </li>
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              Dokumen Pendukung***
            </li>
            <li class="flex items-center capitalize">
              <svg
                class="
                  me-2
                  h-3.5
                  w-3.5
                  flex-shrink-0
                  text-green-500
                  dark:text-green-400
                "
                aria-hidden="true"
                xmlns="http://www.w3.org/2000/svg"
                fill="currentColor"
                viewBox="0 0 20 20"
              >
                <path
                  d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5Zm3.707 8.207-4 4a1 1 0 0 1-1.414 0l-2-2a1 1 0 0 1 1.414-1.414L9 10.586l3.293-3.293a1 1 0 0 1 1.414 1.414Z"
                />
              </svg>
              Izin Trayek Angkutan****
            </li>
          </ul>
          <div
            class="
              my-4
              space-y-1
              rounded-lg
              bg-gray-100
              p-2
              text-xs text-gray-500
            "
          >
            <p class="font-bold">
              Identitas berbentuk KTP atau Paspor atau KIMS
            </p>
            <p>*Identitas Istri jika sudah menikah</p>
            <p>**Pemohon berstatus Janda/Duda</p>
            <p>****Khusus Pembiayaan Angkutan</p>
            <p class="col-p-2">
              ***Sertifikat/Akta Jual Beli/PBB/Rekening Listrik/Telepon/PAM
            </p>
          </div>
          <div class="flex justify-end">
            <span
              class="
                rounded
                bg-gray-100
                px-2.5
                py-1.5
                text-center text-sm
                font-semibold
                capitalize
                hover:bg-blue-600 hover:text-white
              "
              >Unduh persyaratan</span
            >
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="grid h-max content-center pt-24 pb-48 bg-blue-600/5">
    <div class="container mx-auto mt-12 items-center p-6 sm:mt-16">
      <div class="text-gray-700">
        <span
          class="
            rounded-full
            bg-yellow-400
            px-2.5
            py-1.5
            text-center text-xs
            font-bold
            uppercase
          "
          >Proses</span
        >
        <h1
          class="
            my-2
            mb-4
            text-2xl
            font-bold
            capitalize
            text-blue-600
            drop-shadow
          "
        >
          proses jerha
        </h1>
        <div class="sm:flex justify-between">
          <p class="mb-8 max-w-screen-md leading-relaxed">
            Clipan Finance merupakan anak perusahaan Bank Panin yang menyediakan
            fasilitas pembiayaan mobil baru dengan beragam program pembiayaan
            yang menarik.
          </p>
          <div>
            <button
              href="#"
              class="
                mb-2
                rounded-full
                border border-blue-600
                bg-blue-600
                px-5
                py-2.5
                text-sm
                font-bold
                uppercase
                text-white
                hover:bg-blue-700
                hover:text-yellow-400
                hover:shadow-lg
                hover:shadow-blue-700/50
                focus:z-10 focus:outline-none focus:ring-4 focus:ring-gray-200
              "
            >
              KPM Panin
            </button>
          </div>
        </div>
      </div>
    </div>
    <div
      class="
        flex
        w-full
        overflow-x-auto
        pl-4
        py-0
        sm:-mt-8
        md:mx-auto
        [mask-image:_linear-gradient(to_right,transparent_0,_black_12px,_black_calc(100%-128px),transparent_100%)]
      "
    >
      <div class="flex space-x-4 pb-10">
        <div
          class="
            group
            w-24
            hidden
            sm:inline-block
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        ></div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
        <div
          class="
            group
            w-72
            rounded-xl
            border
            bg-white
            p-6
            text-left
            transition
            duration-200
            hover:border-blue-700
            hover:bg-blue-600
            hover:text-white
            hover:shadow-xl
            hover:shadow-blue-600/50
          "
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            class="h-12 w-12 group-hover:fill-yellow-400"
          >
            <path
              d="M11.7 2.805a.75.75 0 01.6 0A60.65 60.65 0 0122.83 8.72a.75.75 0 01-.231 1.337 49.949 49.949 0 00-9.902 3.912l-.003.002-.34.18a.75.75 0 01-.707 0A50.009 50.009 0 007.5 12.174v-.224c0-.131.067-.248.172-.311a54.614 54.614 0 014.653-2.52.75.75 0 00-.65-1.352 56.129 56.129 0 00-4.78 2.589 1.858 1.858 0 00-.859 1.228 49.803 49.803 0 00-4.634-1.527.75.75 0 01-.231-1.337A60.653 60.653 0 0111.7 2.805z"
            />
            <path
              d="M13.06 15.473a48.45 48.45 0 017.666-3.282c.134 1.414.22 2.843.255 4.285a.75.75 0 01-.46.71 47.878 47.878 0 00-8.105 4.342.75.75 0 01-.832 0 47.877 47.877 0 00-8.104-4.342.75.75 0 01-.461-.71c.035-1.442.121-2.87.255-4.286A48.4 48.4 0 016 13.18v1.27a1.5 1.5 0 00-.14 2.508c-.09.38-.222.753-.397 1.11.452.213.901.434 1.346.661a6.729 6.729 0 00.551-1.608 1.5 1.5 0 00.14-2.67v-.645a48.549 48.549 0 013.44 1.668 2.25 2.25 0 002.12 0z"
            />
            <path
              d="M4.462 19.462c.42-.419.753-.89 1-1.394.453.213.902.434 1.347.661a6.743 6.743 0 01-1.286 1.794.75.75 0 11-1.06-1.06z"
            />
          </svg>

          <h1
            class="
              mt-4
              text-xl
              font-semibold
              capitalize
              text-blue-600
              group-hover:text-white
            "
          >
            1. Simulasi
          </h1>
          <p class="pt-2 text-sm">
            Free and Premium themes, UI Kit's, templates and landing pages built
            with Tailwind CSS, HTML &amp; Next.js.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- slider -->
  <section class="grid h-max content-center bg-blue-600">
    <div
      class="
        container
        mx-auto
        my-12
        flex-row-reverse
        items-center
        gap-12
        p-6
        sm:my-16 sm:flex
      "
    >
      <div class="sm:w-1/2">
        <div class="flex w-full">
          <div class="mb-8 sm:p-4">
            <img
              src="https://clipan-v3.netlify.app/slider-1.png"
              loading="lazy"
              alt="Photo by Kaung Htet"
              class="h-full w-full object-cover object-center"
            />
          </div>
        </div>
      </div>
      <div class="text-center text-white sm:w-1/2 sm:text-left">
        <span
          class="
            rounded-full
            bg-yellow-400
            px-2.5
            py-1.5
            text-center text-xs
            font-bold
            uppercase
            text-black
          "
          >Produk Mobil Baru</span
        >
        <h1 class="my-2 mb-6 text-4xl font-bold capitalize drop-shadow">
          Heading promo mobil baru disini
        </h1>
        <p class="mb-8 leading-relaxed">
          Deskripsi singkat filler text, also known as placeholder text. It
          shares some characteristics of a real written text but is random.
        </p>

        <div class="flex justify-center gap-2 sm:justify-start">
          <a
            href="#"
            class="
              mb-2
              me-2
              rounded-full
              border border-gray-200
              bg-white
              px-5
              py-2.5
              text-sm
              font-medium
              text-gray-900
              hover:bg-gray-100 hover:text-blue-700 hover:shadow-lg
              focus:z-10 focus:outline-none focus:ring-4 focus:ring-gray-200
            "
            >Selengkapnya</a
          >
          <a
            href="#"
            class="
              mb-2
              me-2
              rounded-full
              border border-gray-200
              px-5
              py-2.5
              text-sm
              font-medium
              text-white
              hover:bg-gray-100 hover:text-blue-700 hover:shadow-lg
              focus:z-10 focus:outline-none focus:ring-4 focus:ring-gray-200
            "
            >Simulasi</a
          >
        </div>
      </div>
    </div>
  </section>
</template>
