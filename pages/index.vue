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

          <p class="px-8 sm:px-32">
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
              px-10
              py-5
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
              class="absolute right-3 top-3 h-16 w-16 fill-blue-100"
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
    <section class=" bg-gradient-to-br
            from-blue-500
            to-blue-600 py-32">
      <div class="max-w-screen-lg px-5 mx-auto space-y-12 ">
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
          <div class="col-span-7 mb-10">
            <div>
              <form id="contact-form" method="post" class="space-y-5">
                <div class="sm:flex sm:space-x-6 space-y-8 sm:space-y-0">
                  <div class="sm:w-1/2 text-white">
                    <label
                      for="email"
                      class="block mb-1 text-sm uppercase font-bold"
                      >Domisili</label
                    >
                    <select
                      id="countries"
                      class="
                        bg-black/20
                        border-0
                        text-sm
                        rounded-lg
                        focus:ring-blue-500
                        focus:border-blue-900
                        focus:shadow
                        focus:shadow-lg
                        block
                        w-full
                        p-4
                      "
                    >
                      <option>jabodetabek</option>
                      <option>Makasar, Sulawesi</option>
                    </select>
                    <p
                      id="helper-text-explanation"
                      class="mt-1 text-xs opacity-70"
                    >
                      Sesuai KTP, SIM dan Passpor
                    </p>
                  </div>
                  <div class="sm:w-1/2 text-white">
                    <label
                      for="email"
                      class="block mb-1 text-sm uppercase font-bold"
                      >Asuransi</label
                    >
                    <select
                      id="countries"
                      class="
                        bg-black/20
                        border-0
                        text-sm
                        rounded-lg
                        focus:ring-blue-500
                        focus:border-blue-900
                        focus:shadow
                        focus:shadow-lg
                        block
                        w-full
                        p-4
                      "
                    >
                      <option>Hanya Kehilanggan</option>
                      <option>Semua Kerusakan</option>
                      <option>Gabungan</option>
                    </select>
                    <p
                      id="helper-text-explanation"
                      class="mt-1 text-xs opacity-70"
                    >
                      Lihat penjelasan
                      <a href="" class="text-yellow-400 font-bold">lengkap</a>
                    </p>
                  </div>
                </div>
                <div class="sm:flex sm:space-x-6">
                  <div class="w-full text-white">
                    <label
                      for="email"
                      class="block mb-1 text-sm uppercase font-bold"
                      >Harga Kendaraan</label
                    >
                    <div class="relative">
                      <div
                        class="
                          absolute
                          inset-y-0
                          left-0
                          flex
                          items-center
                          pl-3
                          pointer-events-none
                        "
                      >
                        <svg
                          xmlns="http://www.w3.org/2000/svg"
                          width="32"
                          height="32"
                          viewBox="0 0 24 24"
                        >
                          <g fill="#fff">
                            <path
                              d="m17.966 6.558l-1.83-1.83c-1.545-1.545-2.317-2.318-3.32-2.605c-1.003-.288-2.068-.042-4.197.45l-1.228.283c-1.792.413-2.688.62-3.302 1.233c-.613.614-.82 1.51-1.233 3.302l-.284 1.228c-.491 2.13-.737 3.194-.45 4.197c.288 1.003 1.061 1.775 2.606 3.32l1.83 1.83C9.248 20.657 10.592 22 12.262 22c1.671 0 3.015-1.345 5.704-4.034C20.657 15.277 22 13.933 22 12.262c0-1.67-1.345-3.015-4.034-5.704Z"
                              opacity=".5"
                            />
                            <path
                              d="M11.147 14.328c-.673-.672-.667-1.638-.265-2.403a.75.75 0 0 1 1.04-1.046c.34-.18.713-.276 1.085-.272a.75.75 0 0 1-.014 1.5a.88.88 0 0 0-.609.277c-.387.387-.285.775-.177.884c.11.109.497.21.884-.177c.784-.784 2.138-1.044 3.006-.177c.673.673.667 1.639.264 2.404a.75.75 0 0 1-1.04 1.045a2.201 2.201 0 0 1-1.472.232a.75.75 0 1 1 .302-1.47c.177.037.463-.021.708-.266c.388-.388.286-.775.177-.884c-.109-.109-.496-.21-.884.177c-.784.784-2.138 1.044-3.005.176Zm-1.126-4.035a2 2 0 1 0-2.828-2.828a2 2 0 0 0 2.828 2.828Z"
                            />
                          </g>
                        </svg>
                      </div>
                      <input
                        type="text"
                        id="email-address-icon"
                        class="
                          bg-black/20
                          border-0
                          text-sm
                          rounded-lg
                          focus:ring-blue-500
                          focus:border-blue-900
                          focus:shadow
                          focus:shadow-lg
                          block
                          w-full
                          p-4
                          pl-12
                          font-bold
                          placeholder:text-white placeholder:opacity-50
                        "
                        placeholder="1.000.000"
                      />
                    </div>
                    <p
                      id="helper-text-explanation"
                      class="mt-1 text-xs opacity-70"
                    >
                      Minimal 200 Juta Rupiah
                    </p>
                  </div>
                </div>
                <div class="sm:flex sm:space-x-6 space-y-8">
                  <div class="w-full text-white">
                    <label
                      for="email"
                      class="block mb-1 text-sm uppercase font-bold"
                      >Uang Muka</label
                    >
                    <div class="flex">
                      <select
                        id="countries"
                        class="
                          border-l border-blue-800
                          bg-black/20
                          border-0
                          text-sm
                          rounded-l-lg
                          focus:ring-blue-500
                          focus:border-blue-900
                          focus:shadow
                          focus:shadow-lg
                          block
                          w-2/5
                          sm:w-1/5
                          p-4
                        "
                      >
                        <option>20%</option>
                        <option>30%</option>
                      </select>
                      <input
                        type="email"
                        id="email"
                        aria-describedby="helper-text-explanation"
                        class="
                          border-l border-blue-600
                          bg-black/20
                          border-0
                          text-sm
                          rounded-r-lg
                          focus:ring-blue-500
                          focus:border-blue-900
                          focus:shadow
                          focus:shadow-lg
                          block
                          w-3/5
                          sm:w-4/5
                          p-4
                          font-bold
                          placeholder:text-white placeholder:opacity-50
                        "
                        placeholder="213123"
                      />
                    </div>

                    <p
                      id="helper-text-explanation"
                      class="mt-1 text-xs opacity-70"
                    >
                      Minimal Uang muka 15%, maksimal 75%
                    </p>
                  </div>
                </div>

                <button
                  type="submit"
                  class="
                    rounded-full
                    bg-gray-300
                    py-3
                    px-8
                    text-center
                    font-semibold
                    text-white
                    shadow-black
                    transition-all
                    hover:bg-accent-dark
                  "
                  id="contact-form-submit"
                >
                  Submit
                </button>

                <div
                  id="contact-form-notice"
                  class="
                    relative
                    mt-4
                    hidden
                    rounded-lg
                    border border-transparent
                    p-4
                  "
                ></div>
              </form>
            </div>
          </div>

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

            <div class="bg-gray-100 rounded-t-lg p-4 pb-2 sm:px-10">
              <div class="text-center mb-2">
                <h3 class="mb-4 font-bold text-blue-600 text-lg">Simulasi Kredit</h3>
              </div>
              <div class="grid grid-cols-3 content-center">
                <p class="font-bold text-sm">Tenor</p>
                <p class="font-bold text-center text-sm">Total DP</p>
                <p class="font-bold text-right text-sm">Angsuran</p>
              </div>
            </div>
            <div class="p-4 ">
             <div
              v-for="n in 5"
              class="
                grid grid-cols-3
                content-center
                py-4
                sm:px-2
                border-b
                hover:text-blue-600
                hover:bg-gray-100
              "
            >
              <div class="flex items-center content-center">
                <input
                  id="bordered-radio-1"
                  type="radio"
                  value=""
                  name="bordered-radio"
                  class="
                    w-4
                    h-4
                    mr-2
                    bg-gray-100
                    border-gray-300
                    focus:ring-blue-500 focus:ring-2
                  "
                />
                <p class="text-sm">1 Tahun</p>
              </div>
              <div class="text-sm"><p class="text-center">80.000.000</p></div>
              <div class="text-sm"><p class="text-right">6.000.000</p></div>
            </div>
            <div class="mt-6 flex items-center space-x-2">
              <input
                type="checkbox"
                id="contact-form-consent-input"
                name="agree-to-terms"
                class="
                  h-5
                  w-5
                  self-start
                  rounded
                  border-jacarta-200
                  text-accent
                  checked:bg-accent
                 
                "
              />
              <div
                for="contact-form-consent-input"
                class="text-sm"
              >
                <p>Harga tidak mengikat, namun sangat mendekati sampai 85%</p>
               
              </div>
            </div>
            <button
              type="button"
              class="
                mt-5
                text-white
                bg-blue-700
                hover:bg-blue-800
                focus:ring-4 focus:ring-blue-300
                font-medium
                rounded-lg
                text-sm
                px-5
                py-2.5
                mr-2
                mb-2
                dark:bg-blue-600 dark:hover:bg-blue-700
                focus:outline-none
                dark:focus:ring-blue-800
              "
            >
              Default
            </button>
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
