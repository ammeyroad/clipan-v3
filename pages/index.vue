<template>
  <div class="">
    <SliderUtama />
    <HomeKuning />
   
    <!-- sejarah singkat -->
   <SejarahSingkat />

    <!-- Simulasi -->
    <section class="bg-gradient-to-br from-blue-500 to-blue-600 py-32">
      <div class="max-w-screen-lg px-5 mx-auto space-y-12">
        <div class="text-left">
          <p class="font-semibold text-white text-sm xl:text-xl"></p>
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
          <h3 class="text-white text-2xl pt-2 font-bold md:text-4xl">
            Simulasi Kredit
          </h3>
          <garis />

          <p class="text-white sm:pr-32 sm:px-0">
            Berawal dari marketplace lalu tumbuh menjadi platform yang
            memberikan banyak kemudahan untuk berbisnis.
          </p>
        </div>

        <div class="grid grid-cols-1 sm:gap-10 sm:grid-cols-12">
          <!-- simulasi -->
          <div class="col-span-7 mb-10">
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

    <!-- berita terbaru -->
    <section>
      <div class="max-w-screen-lg px-5 mx-auto space-y-12 py-32">
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
          <h3 class="text-blue-600 text-2xl pt-2 font-bold md:text-4xl">
            Perusahaan Clipan
          </h3>
          <garis />

          <p class="pr-8 sm:px-32">
            Berawal dari marketplace lalu tumbuh menjadi platform yang
            memberikan banyak kemudahan untuk berbisnis. Inilah kami, Buka,
            perusahaan yang terus berevolusi dan berinovasi untuk kepentingan
            bersama.
          </p>
        </div>

        <div class="grid grid-cols-1 gap-4 sm:grid-cols-3">
          <div
            class="
              w-full
              
              snap-center
              block
              rounded-2xl
              border border-jacarta-100
              bg-white
              hover:bg-blue-600
              p-2
              text-gray-600
              hover:text-white
              transition-shadow
              hover:shadow-lg
            "
          >
            <figure class="relative">
              <a href="item.html">
                <img
                  src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
                  alt="item 5"
                  class="h-72 w-full rounded-[0.625rem]"
                  loading="lazy"
                />
              </a>
              <div
                class="
                  absolute
                  top-3
                  left-3
                  flex
                  items-center
                  space-x-1
                  rounded-md
                  bg-white
                  p-2
                "
              >
                <span class="text-sm text-blue-600">Mobil Baru</span>
              </div>
            </figure>
            <div class="p-2">
              <div class="mt-4 items-center justify-between">
                <a href="item.html">
                  <span class="font-bold text-lg capitalize line-clamp-2">
                    The biggest moves in NFTs, Bitcoin, crypto rules</span
                  >
                </a>
                <p class="line-clamp-4 mt-2 text-sm">
                  Berawal dari marketplace lalu tumbuh menjadi platform yang
                  memberikan banyak kemudahan untuk berbisnis. Inilah kami,
                  Buka, perusahaan yang
                </p>
                <p class="text-right pt-8">Selengkapnya >></p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style>
.kunings {
  position: absolute;
  right: 0;
  left: 0;
  text-align: center;
}
</style>
