<template>
  <div class="">
    <SliderUtama />

    <section class="relative -mt-24">
      <div class="container kunings w-full">
        <!-- Statistics -->
        <div
          class="
            mb-24
            overflow-hidden
            mx-auto
            max-w-screen-md
            rounded-xl
            border-2 border-yellow-400
            bg-gradient-to-br
            from-yellow-400
            to-yellow-500
            shadow-md
          "
        >
          <div class="grid grid-cols-2 md:grid-cols-4">
            <div
              class="
                py-5
                sm:py-12
                text-center
                align-middle
                duration-300
                hover:scale-110 hover:bg-black/5
              "
            >
              <p class="px-5 sm:px-12">
                <b
                  ><span class="text-5xl">40</span><br />
                  <span class="">tahun telah berdiri</span></b
                >
              </p>
            </div>
            <div
              class="
                py-5
                sm:py-12
                text-center
                align-middle
                duration-300
                hover:scale-110 hover:bg-black/5
              "
            >
              <p class="px-5 sm:px-12" style="text-align: center">
                <b
                  ><span class="text-5xl">63</span><br />
                  <span class="">cabang di indonesia</span></b
                >
              </p>
            </div>
            <div
              class="
                py-5
                sm:py-12
                text-center
                align-middle
                duration-300
                hover:scale-110 hover:bg-black/5
              "
            >
              <p class="px-5 sm:px-12" style="text-align: center">
                <b
                  ><span class="text-5xl">7T</span><br />
                  <span class="">total triliun aset</span></b
                >
              </p>
            </div>
            <div
              class="
                py-5
                sm:py-12
                text-center
                align-middle
                duration-300
                hover:scale-110 hover:bg-black/5
              "
            >
              <p class="px-5 sm:px-12" style="text-align: center">
                <b
                  ><span class="text-5xl">3K</span><br />
                  <span class="">lebih karyawan</span></b
                >
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- sejarah singkat -->
    <section>
      <div class="max-w-screen-lg px-5 mx-auto space-y-12 mb-48">
        <div class="pt-96 sm:text-center text-left">
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
        
        <div class="grid grid-cols-1 gap-5 sm:grid-cols-2">
          <div
            v-for="n in 4"
            class="
              relative
              rounded-xl
              border
              bg-white
              p-5
              shadow-[0_5px_0_0_#10b981]
              transition-shadow
              hover:shadow-[0_16px_24px_-8px_rgba(16,185,129,.3)]
            "
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              width="24"
              height="24"
              class="absolute right-3 top-2 h-16 w-16 fill-blue-100"
            >
              <path fill="none" d="M0 0h24v24H0z"></path>
              <path
                d="M22 6h-7a6 6 0 1 0 0 12h7v2a1 1 0 0 1-1 1H3a1 1 0 0 1-1-1V4a1 1 0 0 1 1-1h18a1 1 0 0 1 1 1v2zm-7 2h8v8h-8a4 4 0 1 1 0-8zm0 3v2h3v-2h-3z"
              ></path>
            </svg>

            <p class="font-bold text-sm text-yellow-500">Kredit</p>
            <h3 class="mb-4 font-bold text-xl">Mobil Baru</h3>
            <p class="">
              Once you've set up your wallet of choice, connect it to OpenSeaby
              clicking the NFT Marketplacein the top right corner.
            </p>
          </div>
        </div>
      </div>
    </section>

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
