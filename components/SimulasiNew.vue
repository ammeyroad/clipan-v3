<template>
  <div>
    <!-- form -->
    <form id="contact-form" method="post" class="space-y-5">
      <!-- domisili -->
      <div class="sm:flex sm:space-x-6 space-y-8 sm:space-y-0">
        <div class="sm:w-1/2 text-white">
          <label for="email" class="block mb-1 text-sm uppercase font-bold"
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
          <p id="helper-text-explanation" class="mt-1 text-xs opacity-70">
            Sesuai KTP, SIM dan Passpor
          </p>
        </div>
        <div class="sm:w-1/2 text-white">
          <label for="email" class="block mb-1 text-sm uppercase font-bold"
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
          <p id="helper-text-explanation" class="mt-1 text-xs opacity-70">
            Lihat penjelasan
            <a href="" class="text-yellow-400 font-bold">lengkap</a>
          </p>
        </div>
      </div>
      <!-- harga otr -->
      <div class="sm:flex sm:space-x-6">
        <div class="w-full text-white">
          <label for="email" class="block mb-1 text-sm uppercase font-bold"
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
          <p id="helper-text-explanation" class="mt-1 text-xs opacity-70">
            Minimal 200 Juta Rupiah
          </p>
        </div>
      </div>
      <!-- uang muka -->
      <div class="sm:flex sm:space-x-6 space-y-8">
        <div class="w-full text-white">
          <label for="email" class="block mb-1 text-sm uppercase font-bold"
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

          <p id="helper-text-explanation" class="mt-1 text-xs opacity-70">
            Minimal Uang muka 15%, maksimal 75%
          </p>
        </div>
      </div>
      <!-- button -->
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
        Ajukan Sekarang
      </button>

      <div
        id="contact-form-notice"
        class="relative mt-4 hidden rounded-lg border border-transparent p-4"
      ></div>
    </form>
  </div>
</template>
