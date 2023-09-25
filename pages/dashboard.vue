<template>
  <div class="mx-auto max-w-screen-xl">
    <div class="flex gap-10 p-5 h-48">
      <div class="w-8/12">
        <div
          class="
            bg-blue-600
            rounded-xl
            flex
            items-center
            justify-between
            p-5
            mb-8
          "
        >
          <div class="flex gap-4 items-center">
            <div>
              <img
                src="https://tairo.cssninja.io/img/avatars/2.svg"
                class="rounded-full w-32"
              />
            </div>
            <div class="text-white">
              <p class="capitalize text-sm">Selamat Datang</p>
              <p class="capitalize font-bold text-xl mt-2">
                rachmat alpriansya
              </p>
              <p class="capitalize text-sm font-bold">1234567890123</p>
            </div>
          </div>
          <div class="bg-white p-8 rounded-lg shadow-xl px-12">
            <p class="capitalize font-bold text-4xl">32</p>
            <p class="capitalize text-sm">angsuran <br />tersisa</p>
          </div>
        </div>
        <div>
          <h4 class="uppercase font-bold text-md text-blue-600 mb-2">
            Detail Kredit
          </h4>

          <div class="grid grid-cols-4 gap-4">
            <div class="col-span-2 p-5 bg-white">
              <div class="flex gap-4 items-top justify-between w-full">
                <div>
                  <img
                    src="https://tairo.cssninja.io/img/avatars/2.svg"
                    class="rounded-full w-12"
                  />
                </div>
                <div>
                  <p class="capitalize text-sm">Tipe Kendaraan</p>
                  <p class="capitalize font-semibold text-xl">
                    All New Avanza Velos CVT Type
                  </p>
                </div>
              </div>
            </div>
            <div class="p-5 bg-white">
              <div>
                <p class="capitalize text-sm">Merek</p>
                <p class="capitalize font-semibold text-xl">Toyota</p>
              </div>
            </div>
            <div class="p-5 bg-white">
              <div>
                <p class="capitalize text-sm">Tahun</p>
                <p class="capitalize font-semibold text-xl">Late 2023</p>
              </div>
            </div>
          </div>
           <div class="grid grid-cols-4 gap-4 mt-4">
            <div class="p-5 bg-white">
              <div>
                  <p class="capitalize text-sm">OTR Kendaraan</p>
                  <p class="capitalize font-semibold text-xl">
                   420.000.000
                  </p>
                </div>
            </div>
            <div class="p-5 bg-white">
              <div>
                <p class="capitalize text-sm">Uang Muka</p>
                <p class="capitalize font-semibold text-xl">46.500.000</p>
              </div>
            </div>
            <div class="p-5 bg-white">
              <div>
                <p class="capitalize text-sm">Angsuran</p>
                <p class="capitalize font-semibold text-xl">6.500.000</p>
              </div>
            </div>
            <div class="p-5 bg-white">
              <div>
                <p class="capitalize text-sm">Tenor</p>
                <p class="capitalize font-semibold text-xl">48 Bulan</p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="w-4/12 sticky fixed">
        <div class="bg-white rounded-xl flex-col p-5">
          <p class="capitalize font-bold text-blue-600 mb-4">
            ringkasan Kredit
          </p>
          <div
            class="
              bg-blue-500
              w-full
              p-8
              rounded-[25px]
              shadow-xl
              px-8
              mb-4
              text-white
            "
          >
            <p class="capitalize text-sm">Tagihan</p>
            <p class="capitalize font-bold text-3xl py-3">Rp 6,500,000</p>
            <div class="flex items-end justify-between">
              <div>
                <p class="capitalize text-xs mt-8">Angsuran ke</p>
                <p class="capitalize text-sm">23 dari 48 Bulan</p>
              </div>
              <div class="text-right">
                <p class="capitalize text-sm">h-5</p>
                <p class="capitalize text-xs">jatuh tempo</p>
              </div>
            </div>
          </div>
          <div>
            <div class="flex items-end justify-between px-5 py-2">
              <div>
                <p class="capitalize text-sm font-bold">Status</p>
              </div>
              <div>
                <p class="capitalize text-sm">Belom terbayar</p>
              </div>
            </div>
            <div class="flex items-end justify-between px-5 py-2">
              <div>
                <p class="capitalize text-sm font-bold">Jatuh Tempo</p>
              </div>
              <div>
                <p class="capitalize text-sm">21 Januari</p>
              </div>
            </div>
            <div class="flex items-end justify-between px-5 py-2">
              <div>
                <p class="capitalize text-sm font-bold">Denda</p>
              </div>
              <div>
                <p class="capitalize text-sm">0</p>
              </div>
            </div>
            <div class="flex items-end justify-between px-5 py-2">
              <div>
                <p class="capitalize text-sm font-bold">Produk</p>
              </div>
              <div>
                <p class="capitalize text-sm">Mobil Bekas</p>
              </div>
            </div>
          </div>
          <div class="border-dashed border-b my-5 border-gray-600 ..."></div>
          <div class="flex items-end justify-between px-5 py-2">
            <div>
              <p class="capitalize text-sm font-bold">total Tagihan</p>
            </div>
            <div>
              <p class="capitalize text-sm">6,500,000</p>
            </div>
          </div>
          <button
            class="
              capitalize
              text-sm
              font-bold
              bg-blue-500
              w-full
              text-center
              p-5
              rounded-lg
              mt-4
              shadow-lg
              text-white
            "
          >
            Bayar Sekarang
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
