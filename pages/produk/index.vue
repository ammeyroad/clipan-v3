<template>
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
        <h1
          class="
            my-2
            mb-6
            text-4xl text-white
            font-bold
            capitalize
            drop-shadow-
          "
        >
          slider_judul disini
        </h1>
        <p class="mb-8">
          slider_deskripsi filler text, also known as placeholder text. It
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
            >slider_link</a
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

  <!-- penjelasan -->
  <section class="grid h-max content-center">
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
            >produk_section</span
          >
          <h1
            class="
              my-2
              mb-6
              text-3xl
              font-bold
              capitalize
              text-blue-600
              drop-shadow-sm
            "
          >
            produk_judul disini
          </h1>
          <p class="mx-auto mb-8 max-w-screen-md">
            produk_deskripsi merupakan anak perusahaan Bank Panin yang
            menyediakan fasilitas pembiayaan mobil baru dengan beragam program
            pembiayaan yang menarik.
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
            grid grid-cols-2
            divide-x divide-y divide-gray-100
            hover:border-1
            sm:grid-cols-4
            lg:divide-y-0
            xl:grid-cols-4
          "
        >
          <div
            class="
              group
              transition
              rounded-xl
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-lg
              hover:shadow-blue-600/50
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
                  feature_judul
                </h5>
                <p class="text-sm">
                  feature_deskripsi, fugiat non cum doloribus aperiam voluptates
                  nostrum.
                </p>
              </div>
            </div>
          </div>
          <div
            class="
              group
              transition
              rounded-xl
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-lg
              hover:shadow-blue-600/50
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
              transition
              rounded-xl
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-lg
              hover:shadow-blue-600/50
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
              transition
              rounded-xl
              hover:z-[1]
              hover:bg-blue-600
              hover:text-white
              hover:shadow-lg
              hover:shadow-blue-600/50
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
  <section class="grid h-max content-center">
    <div class="container mx-auto items-center p-6">
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
  <section class="-mt-44 grid h-max content-center bg-blue-600 py-32">
    <div
      class="container mx-auto mt-32 items-center gap-12 p-6 sm:my-16 sm:flex"
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

  <section class="py-24">
    <div class="grid sm:grid-cols-5 gap-16 sm:px-10 p-8 container mx-auto">
      <div class="sm:col-span-2">
        <div
          class="
            hover:shadow-blue-600/50/50
            rounded-xl
            border
            bg-gray-50
            duration-200
            hover:shadow-lg hover:shadow-blue-600/50
          "
        >
          <div
            class="items-bottom justify-between rounded-t-xl bg-blue-600 py-5"
          >
            <h4
              class="
                mx-auto
                -mt-2
                text-center text-xl
                font-bold
                uppercase
                text-white
              "
            >
              simulasi_judul
            </h4>
            <p class="mx-auto px-10 text-center text-sm capitalize text-white">
              simulasi_deskripsi berikut hal-hal dasar yang menjadi acuan untuk
              simulasi kredit mobil baru :
            </p>
          </div>
          <div class="px-4">
            <div
              class="
                flex
                items-center
                justify-between
                border-b border-dashed
                px-2
                py-4
              "
            >
              <p class="text-sm font-semibold">detail_judul</p>
              <p class="text-right text-sm font-semibold text-blue-600">
                detail_konten
              </p>
            </div>
            <div
              class="
                flex
                items-center
                justify-between
                border-b border-dashed
                px-2
                py-4
              "
            >
              <p class="text-sm font-semibold">Bunga perTahun</p>
              <p class="text-right text-sm font-semibold text-blue-600">2,8%</p>
            </div>
            <div
              class="
                flex
                items-center
                justify-between
                border-b border-dashed
                px-2
                py-4
              "
            >
              <p class="w-1/2 text-sm font-semibold">Tenor</p>
              <p class="w-1/2 text-right text-sm font-semibold text-blue-600">
                1 - 4 Tahun
              </p>
            </div>
            <div
              class="
                flex
                items-center
                justify-between
                border-b border-dashed
                px-2
                py-4
              "
            >
              <p class="w-1/2 text-sm font-semibold">Max Pinjaman</p>
              <p class="w-1/2 text-right text-sm font-semibold text-blue-600">
                500 Juta
              </p>
            </div>
            <div
              class="
                flex
                items-center
                justify-between
                border-b border-dashed
                px-2
                py-4
              "
            >
              <p class="w-1/2 text-sm font-semibold">Max Pinjaman</p>
              <p class="w-1/2 text-right text-sm font-semibold text-blue-600">
                500 Juta
              </p>
            </div>
            <div
              class="
                flex
                items-center
                justify-between
                border-b border-dashed
                px-2
                py-4
              "
            >
              <p class="w-1/2 text-sm font-semibold">Max Pinjaman</p>
              <p class="w-1/2 text-right text-sm font-semibold text-blue-600">
                500 Juta
              </p>
            </div>
            <div class="flex items-center justify-between px-2 py-4 font-bold">
              <p class="w-1/2 text-sm font-semibold">Cashback</p>
              <p class="w-1/2 text-right text-sm font-semibold text-blue-600">
                2.500.000
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="sm:col-span-3">
        <div class="mb-5 text-left">
          <p class="text-sm font-semibold xl:text-xl"></p>
          <span
            class="
              mr-2
              rounded-xl
              bg-yellow-400
              px-2.5
              py-1.5
              text-xs
              font-medium
              text-black
            "
            >simulasi_section</span
          >
          <h3 class="pt-2 text-xl font-bold md:text-2xl">
            Simulasi Mobil Baru
          </h3>
          <garis />
        </div>
        <form id="contact-form" method="post" class="space-y-4">
          <!-- domisili -->
          <div class="space-y-6 sm:flex sm:space-x-4 sm:space-y-0">
            <div class="sm:w-1/2">
              <label
                for="email"
                class="mb-1 block text-sm font-bold uppercase text-blue-600"
                >Domisili</label
              >
              <select
                id="countries"
                class="
                  block
                  w-full
                  rounded-lg
                  border-0
                  bg-slate-50
                  p-4
                  text-sm
                  hover:shadow-lg hover:shadow-blue-600/50
                  focus:border-blue-900 focus:shadow focus:ring-blue-500
                "
              >
                <option>jabodetabek</option>
                <option>Makasar, Sulawesi</option>
              </select>
              <p id="helper-text-explanation" class="mt-1 text-xs opacity-70">
                Sesuai KTP, SIM dan Passpor
              </p>
            </div>
            <div class="sm:w-1/2">
              <label
                for="email"
                class="mb-1 block text-sm font-bold uppercase text-blue-600"
                >Asuransi</label
              >
              <select
                id="countries"
                class="
                  block
                  w-full
                  rounded-lg
                  border-0
                  bg-slate-50
                  p-4
                  text-sm
                  hover:shadow-lg hover:shadow-blue-600/50
                  focus:border-blue-900 focus:shadow focus:ring-blue-500
                "
              >
                <option>Hanya Kehilanggan</option>
                <option>Semua Kerusakan</option>
                <option>Gabungan</option>
              </select>
              <p id="helper-text-explanation" class="mt-1 text-xs opacity-70">
                Lihat penjelasan
                <a href="" class="font-bold text-yellow-400">lengkap</a>
              </p>
            </div>
          </div>
          <!-- harga otr -->
          <div class="sm:flex sm:space-x-6">
            <div class="w-full">
              <label
                for="email"
                class="mb-1 block text-sm font-bold uppercase text-blue-600"
                >Harga Kendaraan</label
              >
              <div class="relative">
                <div
                  class="
                    pointer-events-none
                    absolute
                    inset-y-0
                    left-0
                    flex
                    items-center
                    pl-3
                  "
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="32"
                    height="32"
                    viewBox="0 0 24 24"
                    class="fill-blue-600"
                  >
                    <g fill="">
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
                    placeholder
                    block
                    w-full
                    rounded-lg
                    border-0
                    bg-slate-50
                    p-4
                    pl-12
                    text-sm
                    font-bold
                    placeholder:opacity-50
                    hover:shadow-lg hover:shadow-blue-600/50
                    focus:border-blue-900 focus:shadow focus:ring-blue-500
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
          <div class="space-y-8 sm:flex sm:space-x-6">
            <div class="w-full">
              <label
                for="email"
                class="mb-1 block text-sm font-bold uppercase text-blue-600"
                >Uang Muka</label
              >
              <div class="flex gap-0.5">
                <select
                  id="countries"
                  class="
                    border-
                    block
                    w-1/5
                    rounded-l-lg
                    border-0 border-blue-800
                    bg-slate-50
                    p-4
                    text-sm
                    hover:shadow-lg hover:shadow-blue-600/50
                    focus:border-blue-900 focus:shadow focus:ring-blue-500
                    sm:w-1/5
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
                    placeholder
                    block
                    w-4/5
                    rounded-r-lg
                    border-0 border-white
                    bg-slate-50
                    p-4
                    text-sm
                    font-bold
                    placeholder:opacity-50
                    hover:shadow-lg hover:shadow-blue-600/50
                    focus:border-blue-900 focus:shadow focus:ring-blue-500
                    sm:w-4/5
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
            href="#"
            class="
              mb-2
              scale-100
              rounded-full
              border border-blue-600
              bg-blue-600
              px-5
              py-2.5
              text-sm
              font-bold
              uppercase
              text-white
              transition
              duration-150
              hover:scale-105
              hover:bg-blue-700
              hover:text-yellow-400
              hover:shadow-lg
              hover:shadow-blue-700/50
              focus:z-10 focus:outline-none focus:ring-4 focus:ring-gray-200
            "
          >
            <div class="flex items-center gap-2">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
                class="h-4 w-4"
              >
                <path
                  fill-rule="evenodd"
                  d="M6.32 1.827a49.255 49.255 0 0111.36 0c1.497.174 2.57 1.46 2.57 2.93V19.5a3 3 0 01-3 3H6.75a3 3 0 01-3-3V4.757c0-1.47 1.073-2.756 2.57-2.93zM7.5 11.25a.75.75 0 01.75-.75h.008a.75.75 0 01.75.75v.008a.75.75 0 01-.75.75H8.25a.75.75 0 01-.75-.75v-.008zm.75 1.5a.75.75 0 00-.75.75v.008c0 .414.336.75.75.75h.008a.75.75 0 00.75-.75V13.5a.75.75 0 00-.75-.75H8.25zm-.75 3a.75.75 0 01.75-.75h.008a.75.75 0 01.75.75v.008a.75.75 0 01-.75.75H8.25a.75.75 0 01-.75-.75v-.008zm.75 1.5a.75.75 0 00-.75.75v.008c0 .414.336.75.75.75h.008a.75.75 0 00.75-.75V18a.75.75 0 00-.75-.75H8.25zm1.748-6a.75.75 0 01.75-.75h.007a.75.75 0 01.75.75v.008a.75.75 0 01-.75.75h-.007a.75.75 0 01-.75-.75v-.008zm.75 1.5a.75.75 0 00-.75.75v.008c0 .414.335.75.75.75h.007a.75.75 0 00.75-.75V13.5a.75.75 0 00-.75-.75h-.007zm-.75 3a.75.75 0 01.75-.75h.007a.75.75 0 01.75.75v.008a.75.75 0 01-.75.75h-.007a.75.75 0 01-.75-.75v-.008zm.75 1.5a.75.75 0 00-.75.75v.008c0 .414.335.75.75.75h.007a.75.75 0 00.75-.75V18a.75.75 0 00-.75-.75h-.007zm1.754-6a.75.75 0 01.75-.75h.008a.75.75 0 01.75.75v.008a.75.75 0 01-.75.75h-.008a.75.75 0 01-.75-.75v-.008zm.75 1.5a.75.75 0 00-.75.75v.008c0 .414.336.75.75.75h.008a.75.75 0 00.75-.75V13.5a.75.75 0 00-.75-.75h-.008zm-.75 3a.75.75 0 01.75-.75h.008a.75.75 0 01.75.75v.008a.75.75 0 01-.75.75h-.008a.75.75 0 01-.75-.75v-.008zm.75 1.5a.75.75 0 00-.75.75v.008c0 .414.336.75.75.75h.008a.75.75 0 00.75-.75V18a.75.75 0 00-.75-.75h-.008zm1.748-6a.75.75 0 01.75-.75h.008a.75.75 0 01.75.75v.008a.75.75 0 01-.75.75h-.008a.75.75 0 01-.75-.75v-.008zm.75 1.5a.75.75 0 00-.75.75v.008c0 .414.336.75.75.75h.008a.75.75 0 00.75-.75V13.5a.75.75 0 00-.75-.75h-.008zm-8.25-6A.75.75 0 018.25 6h7.5a.75.75 0 01.75.75v.75a.75.75 0 01-.75.75h-7.5a.75.75 0 01-.75-.75v-.75zm9 9a.75.75 0 00-1.5 0V18a.75.75 0 001.5 0v-2.25z"
                  clip-rule="evenodd"
                />
              </svg>

              <p>simulasikan</p>
            </div>
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
  </section>
  <section class="grid h-max content-center">
    <div class="container mx-auto items-center px-6 p-6">
      <div class="text-gray-700">
        <div class="sm:flex justify-between items-end">
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
              kendaraan of the month
            </h1>
          </div>
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
              lihat semua
            </button>
          </div>
        </div>
      </div>
      <div class="py-8">
        <div
          class="
            flex
            w-full
            overflow-x-auto
            pl-4
            py-0
            sm:-mt-8
            md:mx-auto
            [mask-image:_linear-gradient(to_right,transparent_0,_black_128px,_black_calc(100%-128px),transparent_100%)]
          "
        >
          <div class="flex space-x-4 pb-10 animate-infinitescroll">
            ">
            <div class="rounded-xl w-80 bg-white p-2">
              <a
                href="#"
                class="
                  group
                  relative
                  mb-2
                  block
                  h-72
                  overflow-hidden
                  rounded-lg
                  bg-gray-100
                  lg:mb-3
                "
              >
                <img
                  src="https://images.unsplash.com/photo-1552374196-1ab2a1c593e8?auto=format&q=75&fit=crop&crop=top&w=600&h=700"
                  loading="lazy"
                  alt="Photo by Austin Wade"
                  class="
                    h-full
                    w-full
                    object-cover object-center
                    transition
                    duration-200
                    group-hover:scale-110
                  "
                />

                <div class="absolute left-2 top-2 flex gap-2">
                  <span
                    class="
                      rounded
                      bg-white
                      px-3
                      py-1.5
                      text-sm
                      font-bold
                      uppercase
                      tracking-wider
                      text-gray-800
                    "
                    >Mobil baru</span
                  >
                </div>
              </a>

              <div class="flex items-start justify-between gap-2 px-2">
                <div class="w-10/12 pr-4">
                  <a
                    href="#"
                    class="
                      font-bold
                      capitalize
                      text-gray-800
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                    >produk_judul 2018 Mercedes-Benz GLA 200 AMG 1.6</a
                  >
                </div>

                <div class="w-2/12">
                  <img
                    alt="testimonial"
                    class="
                      mx-auto
                      inline-block
                      h-16
                      w-16
                      rounded-full
                      border-white
                      object-cover object-center
                    "
                    src="https://wickedblocks.dev/assets/images/avatar.png"
                  />
                </div>
              </div>
              <div class="text-semibold mt-4 flex gap-2 text-xs text-gray-400">
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M8.161 2.58a1.875 1.875 0 011.678 0l4.993 2.498c.106.052.23.052.336 0l3.869-1.935A1.875 1.875 0 0121.75 4.82v12.485c0 .71-.401 1.36-1.037 1.677l-4.875 2.437a1.875 1.875 0 01-1.676 0l-4.994-2.497a.375.375 0 00-.336 0l-3.868 1.935A1.875 1.875 0 012.25 19.18V6.695c0-.71.401-1.36 1.036-1.677l4.875-2.437zM9 6a.75.75 0 01.75.75V15a.75.75 0 01-1.5 0V6.75A.75.75 0 019 6zm6.75 3a.75.75 0 00-1.5 0v8.25a.75.75 0 001.5 0V9z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">123.000 km</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.828 2.25c-.916 0-1.699.663-1.85 1.567l-.091.549a.798.798 0 01-.517.608 7.45 7.45 0 00-.478.198.798.798 0 01-.796-.064l-.453-.324a1.875 1.875 0 00-2.416.2l-.243.243a1.875 1.875 0 00-.2 2.416l.324.453a.798.798 0 01.064.796 7.448 7.448 0 00-.198.478.798.798 0 01-.608.517l-.55.092a1.875 1.875 0 00-1.566 1.849v.344c0 .916.663 1.699 1.567 1.85l.549.091c.281.047.508.25.608.517.06.162.127.321.198.478a.798.798 0 01-.064.796l-.324.453a1.875 1.875 0 00.2 2.416l.243.243c.648.648 1.67.733 2.416.2l.453-.324a.798.798 0 01.796-.064c.157.071.316.137.478.198.267.1.47.327.517.608l.092.55c.15.903.932 1.566 1.849 1.566h.344c.916 0 1.699-.663 1.85-1.567l.091-.549a.798.798 0 01.517-.608 7.52 7.52 0 00.478-.198.798.798 0 01.796.064l.453.324a1.875 1.875 0 002.416-.2l.243-.243c.648-.648.733-1.67.2-2.416l-.324-.453a.798.798 0 01-.064-.796c.071-.157.137-.316.198-.478.1-.267.327-.47.608-.517l.55-.091a1.875 1.875 0 001.566-1.85v-.344c0-.916-.663-1.699-1.567-1.85l-.549-.091a.798.798 0 01-.608-.517 7.507 7.507 0 00-.198-.478.798.798 0 01.064-.796l.324-.453a1.875 1.875 0 00-.2-2.416l-.243-.243a1.875 1.875 0 00-2.416-.2l-.453.324a.798.798 0 01-.796.064 7.462 7.462 0 00-.478-.198.798.798 0 01-.517-.608l-.091-.55a1.875 1.875 0 00-1.85-1.566h-.344zM12 15.75a3.75 3.75 0 100-7.5 3.75 3.75 0 000 7.5z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">AT</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">Jakarta Utara</p>
                </span>
              </div>
              <hr class="my-2" />
              <div class="flex items-end justify-between">
                <div class="px-2">
                  <a
                    href="#"
                    class="
                      text-2xl
                      font-bold
                      capitalize
                      text-blue-600
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                  >
                    3.000.000
                    <span class="text-semibold text-xs text-gray-700"
                      >/bulan
                    </span>
                  </a>
                  <p class="text-xs">Uang muka mulai dari Rp. 23.000.000</p>
                </div>
                <button
                  href="#"
                  class="
                    h-10
                    w-10
                    scale-100
                    rounded-full
                    border border-blue-600
                    bg-transparent
                    text-sm
                    font-bold
                    uppercase
                    text-blue-600
                    transition
                    duration-150
                    hover:scale-105
                    hover:bg-blue-700
                    hover:text-yellow-400
                    hover:shadow-lg
                    hover:shadow-blue-700/50
                    focus:z-10
                    focus:outline-none
                    focus:ring-4
                    focus:ring-gray-200
                  "
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="mx-auto h-6 w-6"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M3.75 12a.75.75 0 01.75-.75h13.19l-5.47-5.47a.75.75 0 011.06-1.06l6.75 6.75a.75.75 0 010 1.06l-6.75 6.75a.75.75 0 11-1.06-1.06l5.47-5.47H4.5a.75.75 0 01-.75-.75z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </button>
              </div>
            </div>
            <div class="rounded-xl w-80 bg-white p-2">
              <a
                href="#"
                class="
                  group
                  relative
                  mb-2
                  block
                  h-72
                  overflow-hidden
                  rounded-lg
                  bg-gray-100
                  lg:mb-3
                "
              >
                <img
                  src="https://images.unsplash.com/photo-1552374196-1ab2a1c593e8?auto=format&q=75&fit=crop&crop=top&w=600&h=700"
                  loading="lazy"
                  alt="Photo by Austin Wade"
                  class="
                    h-full
                    w-full
                    object-cover object-center
                    transition
                    duration-200
                    group-hover:scale-110
                  "
                />

                <div class="absolute left-2 top-2 flex gap-2">
                  <span
                    class="
                      rounded
                      bg-white
                      px-3
                      py-1.5
                      text-sm
                      font-bold
                      uppercase
                      tracking-wider
                      text-gray-800
                    "
                    >Mobil baru</span
                  >
                </div>
              </a>

              <div class="flex items-start justify-between gap-2 px-2">
                <div class="w-10/12 pr-4">
                  <a
                    href="#"
                    class="
                      font-bold
                      capitalize
                      text-gray-800
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                    >produk_judul 2018 Mercedes-Benz GLA 200 AMG 1.6</a
                  >
                </div>

                <div class="w-2/12">
                  <img
                    alt="testimonial"
                    class="
                      mx-auto
                      inline-block
                      h-16
                      w-16
                      rounded-full
                      border-white
                      object-cover object-center
                    "
                    src="https://wickedblocks.dev/assets/images/avatar.png"
                  />
                </div>
              </div>
              <div class="text-semibold mt-4 flex gap-2 text-xs text-gray-400">
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M8.161 2.58a1.875 1.875 0 011.678 0l4.993 2.498c.106.052.23.052.336 0l3.869-1.935A1.875 1.875 0 0121.75 4.82v12.485c0 .71-.401 1.36-1.037 1.677l-4.875 2.437a1.875 1.875 0 01-1.676 0l-4.994-2.497a.375.375 0 00-.336 0l-3.868 1.935A1.875 1.875 0 012.25 19.18V6.695c0-.71.401-1.36 1.036-1.677l4.875-2.437zM9 6a.75.75 0 01.75.75V15a.75.75 0 01-1.5 0V6.75A.75.75 0 019 6zm6.75 3a.75.75 0 00-1.5 0v8.25a.75.75 0 001.5 0V9z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">123.000 km</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.828 2.25c-.916 0-1.699.663-1.85 1.567l-.091.549a.798.798 0 01-.517.608 7.45 7.45 0 00-.478.198.798.798 0 01-.796-.064l-.453-.324a1.875 1.875 0 00-2.416.2l-.243.243a1.875 1.875 0 00-.2 2.416l.324.453a.798.798 0 01.064.796 7.448 7.448 0 00-.198.478.798.798 0 01-.608.517l-.55.092a1.875 1.875 0 00-1.566 1.849v.344c0 .916.663 1.699 1.567 1.85l.549.091c.281.047.508.25.608.517.06.162.127.321.198.478a.798.798 0 01-.064.796l-.324.453a1.875 1.875 0 00.2 2.416l.243.243c.648.648 1.67.733 2.416.2l.453-.324a.798.798 0 01.796-.064c.157.071.316.137.478.198.267.1.47.327.517.608l.092.55c.15.903.932 1.566 1.849 1.566h.344c.916 0 1.699-.663 1.85-1.567l.091-.549a.798.798 0 01.517-.608 7.52 7.52 0 00.478-.198.798.798 0 01.796.064l.453.324a1.875 1.875 0 002.416-.2l.243-.243c.648-.648.733-1.67.2-2.416l-.324-.453a.798.798 0 01-.064-.796c.071-.157.137-.316.198-.478.1-.267.327-.47.608-.517l.55-.091a1.875 1.875 0 001.566-1.85v-.344c0-.916-.663-1.699-1.567-1.85l-.549-.091a.798.798 0 01-.608-.517 7.507 7.507 0 00-.198-.478.798.798 0 01.064-.796l.324-.453a1.875 1.875 0 00-.2-2.416l-.243-.243a1.875 1.875 0 00-2.416-.2l-.453.324a.798.798 0 01-.796.064 7.462 7.462 0 00-.478-.198.798.798 0 01-.517-.608l-.091-.55a1.875 1.875 0 00-1.85-1.566h-.344zM12 15.75a3.75 3.75 0 100-7.5 3.75 3.75 0 000 7.5z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">AT</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">Jakarta Utara</p>
                </span>
              </div>
              <hr class="my-2" />
              <div class="flex items-end justify-between">
                <div class="px-2">
                  <a
                    href="#"
                    class="
                      text-2xl
                      font-bold
                      capitalize
                      text-blue-600
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                  >
                    3.000.000
                    <span class="text-semibold text-xs text-gray-700"
                      >/bulan
                    </span>
                  </a>
                  <p class="text-xs">Uang muka mulai dari Rp. 23.000.000</p>
                </div>
                <button
                  href="#"
                  class="
                    h-10
                    w-10
                    scale-100
                    rounded-full
                    border border-blue-600
                    bg-transparent
                    text-sm
                    font-bold
                    uppercase
                    text-blue-600
                    transition
                    duration-150
                    hover:scale-105
                    hover:bg-blue-700
                    hover:text-yellow-400
                    hover:shadow-lg
                    hover:shadow-blue-700/50
                    focus:z-10
                    focus:outline-none
                    focus:ring-4
                    focus:ring-gray-200
                  "
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="mx-auto h-6 w-6"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M3.75 12a.75.75 0 01.75-.75h13.19l-5.47-5.47a.75.75 0 011.06-1.06l6.75 6.75a.75.75 0 010 1.06l-6.75 6.75a.75.75 0 11-1.06-1.06l5.47-5.47H4.5a.75.75 0 01-.75-.75z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </button>
              </div>
            </div>
            <div class="rounded-xl w-80 bg-white p-2">
              <a
                href="#"
                class="
                  group
                  relative
                  mb-2
                  block
                  h-72
                  overflow-hidden
                  rounded-lg
                  bg-gray-100
                  lg:mb-3
                "
              >
                <img
                  src="https://images.unsplash.com/photo-1552374196-1ab2a1c593e8?auto=format&q=75&fit=crop&crop=top&w=600&h=700"
                  loading="lazy"
                  alt="Photo by Austin Wade"
                  class="
                    h-full
                    w-full
                    object-cover object-center
                    transition
                    duration-200
                    group-hover:scale-110
                  "
                />

                <div class="absolute left-2 top-2 flex gap-2">
                  <span
                    class="
                      rounded
                      bg-white
                      px-3
                      py-1.5
                      text-sm
                      font-bold
                      uppercase
                      tracking-wider
                      text-gray-800
                    "
                    >Mobil baru</span
                  >
                </div>
              </a>

              <div class="flex items-start justify-between gap-2 px-2">
                <div class="w-10/12 pr-4">
                  <a
                    href="#"
                    class="
                      font-bold
                      capitalize
                      text-gray-800
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                    >produk_judul 2018 Mercedes-Benz GLA 200 AMG 1.6</a
                  >
                </div>

                <div class="w-2/12">
                  <img
                    alt="testimonial"
                    class="
                      mx-auto
                      inline-block
                      h-16
                      w-16
                      rounded-full
                      border-white
                      object-cover object-center
                    "
                    src="https://wickedblocks.dev/assets/images/avatar.png"
                  />
                </div>
              </div>
              <div class="text-semibold mt-4 flex gap-2 text-xs text-gray-400">
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M8.161 2.58a1.875 1.875 0 011.678 0l4.993 2.498c.106.052.23.052.336 0l3.869-1.935A1.875 1.875 0 0121.75 4.82v12.485c0 .71-.401 1.36-1.037 1.677l-4.875 2.437a1.875 1.875 0 01-1.676 0l-4.994-2.497a.375.375 0 00-.336 0l-3.868 1.935A1.875 1.875 0 012.25 19.18V6.695c0-.71.401-1.36 1.036-1.677l4.875-2.437zM9 6a.75.75 0 01.75.75V15a.75.75 0 01-1.5 0V6.75A.75.75 0 019 6zm6.75 3a.75.75 0 00-1.5 0v8.25a.75.75 0 001.5 0V9z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">123.000 km</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.828 2.25c-.916 0-1.699.663-1.85 1.567l-.091.549a.798.798 0 01-.517.608 7.45 7.45 0 00-.478.198.798.798 0 01-.796-.064l-.453-.324a1.875 1.875 0 00-2.416.2l-.243.243a1.875 1.875 0 00-.2 2.416l.324.453a.798.798 0 01.064.796 7.448 7.448 0 00-.198.478.798.798 0 01-.608.517l-.55.092a1.875 1.875 0 00-1.566 1.849v.344c0 .916.663 1.699 1.567 1.85l.549.091c.281.047.508.25.608.517.06.162.127.321.198.478a.798.798 0 01-.064.796l-.324.453a1.875 1.875 0 00.2 2.416l.243.243c.648.648 1.67.733 2.416.2l.453-.324a.798.798 0 01.796-.064c.157.071.316.137.478.198.267.1.47.327.517.608l.092.55c.15.903.932 1.566 1.849 1.566h.344c.916 0 1.699-.663 1.85-1.567l.091-.549a.798.798 0 01.517-.608 7.52 7.52 0 00.478-.198.798.798 0 01.796.064l.453.324a1.875 1.875 0 002.416-.2l.243-.243c.648-.648.733-1.67.2-2.416l-.324-.453a.798.798 0 01-.064-.796c.071-.157.137-.316.198-.478.1-.267.327-.47.608-.517l.55-.091a1.875 1.875 0 001.566-1.85v-.344c0-.916-.663-1.699-1.567-1.85l-.549-.091a.798.798 0 01-.608-.517 7.507 7.507 0 00-.198-.478.798.798 0 01.064-.796l.324-.453a1.875 1.875 0 00-.2-2.416l-.243-.243a1.875 1.875 0 00-2.416-.2l-.453.324a.798.798 0 01-.796.064 7.462 7.462 0 00-.478-.198.798.798 0 01-.517-.608l-.091-.55a1.875 1.875 0 00-1.85-1.566h-.344zM12 15.75a3.75 3.75 0 100-7.5 3.75 3.75 0 000 7.5z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">AT</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">Jakarta Utara</p>
                </span>
              </div>
              <hr class="my-2" />
              <div class="flex items-end justify-between">
                <div class="px-2">
                  <a
                    href="#"
                    class="
                      text-2xl
                      font-bold
                      capitalize
                      text-blue-600
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                  >
                    3.000.000
                    <span class="text-semibold text-xs text-gray-700"
                      >/bulan
                    </span>
                  </a>
                  <p class="text-xs">Uang muka mulai dari Rp. 23.000.000</p>
                </div>
                <button
                  href="#"
                  class="
                    h-10
                    w-10
                    scale-100
                    rounded-full
                    border border-blue-600
                    bg-transparent
                    text-sm
                    font-bold
                    uppercase
                    text-blue-600
                    transition
                    duration-150
                    hover:scale-105
                    hover:bg-blue-700
                    hover:text-yellow-400
                    hover:shadow-lg
                    hover:shadow-blue-700/50
                    focus:z-10
                    focus:outline-none
                    focus:ring-4
                    focus:ring-gray-200
                  "
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="mx-auto h-6 w-6"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M3.75 12a.75.75 0 01.75-.75h13.19l-5.47-5.47a.75.75 0 011.06-1.06l6.75 6.75a.75.75 0 010 1.06l-6.75 6.75a.75.75 0 11-1.06-1.06l5.47-5.47H4.5a.75.75 0 01-.75-.75z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </button>
              </div>
            </div>
            <div class="rounded-xl w-80 bg-white p-2">
              <a
                href="#"
                class="
                  group
                  relative
                  mb-2
                  block
                  h-72
                  overflow-hidden
                  rounded-lg
                  bg-gray-100
                  lg:mb-3
                "
              >
                <img
                  src="https://images.unsplash.com/photo-1552374196-1ab2a1c593e8?auto=format&q=75&fit=crop&crop=top&w=600&h=700"
                  loading="lazy"
                  alt="Photo by Austin Wade"
                  class="
                    h-full
                    w-full
                    object-cover object-center
                    transition
                    duration-200
                    group-hover:scale-110
                  "
                />

                <div class="absolute left-2 top-2 flex gap-2">
                  <span
                    class="
                      rounded
                      bg-white
                      px-3
                      py-1.5
                      text-sm
                      font-bold
                      uppercase
                      tracking-wider
                      text-gray-800
                    "
                    >Mobil baru</span
                  >
                </div>
              </a>

              <div class="flex items-start justify-between gap-2 px-2">
                <div class="w-10/12 pr-4">
                  <a
                    href="#"
                    class="
                      font-bold
                      capitalize
                      text-gray-800
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                    >produk_judul 2018 Mercedes-Benz GLA 200 AMG 1.6</a
                  >
                </div>

                <div class="w-2/12">
                  <img
                    alt="testimonial"
                    class="
                      mx-auto
                      inline-block
                      h-16
                      w-16
                      rounded-full
                      border-white
                      object-cover object-center
                    "
                    src="https://wickedblocks.dev/assets/images/avatar.png"
                  />
                </div>
              </div>
              <div class="text-semibold mt-4 flex gap-2 text-xs text-gray-400">
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M8.161 2.58a1.875 1.875 0 011.678 0l4.993 2.498c.106.052.23.052.336 0l3.869-1.935A1.875 1.875 0 0121.75 4.82v12.485c0 .71-.401 1.36-1.037 1.677l-4.875 2.437a1.875 1.875 0 01-1.676 0l-4.994-2.497a.375.375 0 00-.336 0l-3.868 1.935A1.875 1.875 0 012.25 19.18V6.695c0-.71.401-1.36 1.036-1.677l4.875-2.437zM9 6a.75.75 0 01.75.75V15a.75.75 0 01-1.5 0V6.75A.75.75 0 019 6zm6.75 3a.75.75 0 00-1.5 0v8.25a.75.75 0 001.5 0V9z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">123.000 km</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.828 2.25c-.916 0-1.699.663-1.85 1.567l-.091.549a.798.798 0 01-.517.608 7.45 7.45 0 00-.478.198.798.798 0 01-.796-.064l-.453-.324a1.875 1.875 0 00-2.416.2l-.243.243a1.875 1.875 0 00-.2 2.416l.324.453a.798.798 0 01.064.796 7.448 7.448 0 00-.198.478.798.798 0 01-.608.517l-.55.092a1.875 1.875 0 00-1.566 1.849v.344c0 .916.663 1.699 1.567 1.85l.549.091c.281.047.508.25.608.517.06.162.127.321.198.478a.798.798 0 01-.064.796l-.324.453a1.875 1.875 0 00.2 2.416l.243.243c.648.648 1.67.733 2.416.2l.453-.324a.798.798 0 01.796-.064c.157.071.316.137.478.198.267.1.47.327.517.608l.092.55c.15.903.932 1.566 1.849 1.566h.344c.916 0 1.699-.663 1.85-1.567l.091-.549a.798.798 0 01.517-.608 7.52 7.52 0 00.478-.198.798.798 0 01.796.064l.453.324a1.875 1.875 0 002.416-.2l.243-.243c.648-.648.733-1.67.2-2.416l-.324-.453a.798.798 0 01-.064-.796c.071-.157.137-.316.198-.478.1-.267.327-.47.608-.517l.55-.091a1.875 1.875 0 001.566-1.85v-.344c0-.916-.663-1.699-1.567-1.85l-.549-.091a.798.798 0 01-.608-.517 7.507 7.507 0 00-.198-.478.798.798 0 01.064-.796l.324-.453a1.875 1.875 0 00-.2-2.416l-.243-.243a1.875 1.875 0 00-2.416-.2l-.453.324a.798.798 0 01-.796.064 7.462 7.462 0 00-.478-.198.798.798 0 01-.517-.608l-.091-.55a1.875 1.875 0 00-1.85-1.566h-.344zM12 15.75a3.75 3.75 0 100-7.5 3.75 3.75 0 000 7.5z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">AT</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">Jakarta Utara</p>
                </span>
              </div>
              <hr class="my-2" />
              <div class="flex items-end justify-between">
                <div class="px-2">
                  <a
                    href="#"
                    class="
                      text-2xl
                      font-bold
                      capitalize
                      text-blue-600
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                  >
                    3.000.000
                    <span class="text-semibold text-xs text-gray-700"
                      >/bulan
                    </span>
                  </a>
                  <p class="text-xs">Uang muka mulai dari Rp. 23.000.000</p>
                </div>
                <button
                  href="#"
                  class="
                    h-10
                    w-10
                    scale-100
                    rounded-full
                    border border-blue-600
                    bg-transparent
                    text-sm
                    font-bold
                    uppercase
                    text-blue-600
                    transition
                    duration-150
                    hover:scale-105
                    hover:bg-blue-700
                    hover:text-yellow-400
                    hover:shadow-lg
                    hover:shadow-blue-700/50
                    focus:z-10
                    focus:outline-none
                    focus:ring-4
                    focus:ring-gray-200
                  "
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="mx-auto h-6 w-6"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M3.75 12a.75.75 0 01.75-.75h13.19l-5.47-5.47a.75.75 0 011.06-1.06l6.75 6.75a.75.75 0 010 1.06l-6.75 6.75a.75.75 0 11-1.06-1.06l5.47-5.47H4.5a.75.75 0 01-.75-.75z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </button>
              </div>
            </div>
            <div class="rounded-xl w-80 bg-white p-2">
              <a
                href="#"
                class="
                  group
                  relative
                  mb-2
                  block
                  h-72
                  overflow-hidden
                  rounded-lg
                  bg-gray-100
                  lg:mb-3
                "
              >
                <img
                  src="https://images.unsplash.com/photo-1552374196-1ab2a1c593e8?auto=format&q=75&fit=crop&crop=top&w=600&h=700"
                  loading="lazy"
                  alt="Photo by Austin Wade"
                  class="
                    h-full
                    w-full
                    object-cover object-center
                    transition
                    duration-200
                    group-hover:scale-110
                  "
                />

                <div class="absolute left-2 top-2 flex gap-2">
                  <span
                    class="
                      rounded
                      bg-white
                      px-3
                      py-1.5
                      text-sm
                      font-bold
                      uppercase
                      tracking-wider
                      text-gray-800
                    "
                    >Mobil baru</span
                  >
                </div>
              </a>

              <div class="flex items-start justify-between gap-2 px-2">
                <div class="w-10/12 pr-4">
                  <a
                    href="#"
                    class="
                      font-bold
                      capitalize
                      text-gray-800
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                    >produk_judul 2018 Mercedes-Benz GLA 200 AMG 1.6</a
                  >
                </div>

                <div class="w-2/12">
                  <img
                    alt="testimonial"
                    class="
                      mx-auto
                      inline-block
                      h-16
                      w-16
                      rounded-full
                      border-white
                      object-cover object-center
                    "
                    src="https://wickedblocks.dev/assets/images/avatar.png"
                  />
                </div>
              </div>
              <div class="text-semibold mt-4 flex gap-2 text-xs text-gray-400">
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M8.161 2.58a1.875 1.875 0 011.678 0l4.993 2.498c.106.052.23.052.336 0l3.869-1.935A1.875 1.875 0 0121.75 4.82v12.485c0 .71-.401 1.36-1.037 1.677l-4.875 2.437a1.875 1.875 0 01-1.676 0l-4.994-2.497a.375.375 0 00-.336 0l-3.868 1.935A1.875 1.875 0 012.25 19.18V6.695c0-.71.401-1.36 1.036-1.677l4.875-2.437zM9 6a.75.75 0 01.75.75V15a.75.75 0 01-1.5 0V6.75A.75.75 0 019 6zm6.75 3a.75.75 0 00-1.5 0v8.25a.75.75 0 001.5 0V9z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">123.000 km</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.828 2.25c-.916 0-1.699.663-1.85 1.567l-.091.549a.798.798 0 01-.517.608 7.45 7.45 0 00-.478.198.798.798 0 01-.796-.064l-.453-.324a1.875 1.875 0 00-2.416.2l-.243.243a1.875 1.875 0 00-.2 2.416l.324.453a.798.798 0 01.064.796 7.448 7.448 0 00-.198.478.798.798 0 01-.608.517l-.55.092a1.875 1.875 0 00-1.566 1.849v.344c0 .916.663 1.699 1.567 1.85l.549.091c.281.047.508.25.608.517.06.162.127.321.198.478a.798.798 0 01-.064.796l-.324.453a1.875 1.875 0 00.2 2.416l.243.243c.648.648 1.67.733 2.416.2l.453-.324a.798.798 0 01.796-.064c.157.071.316.137.478.198.267.1.47.327.517.608l.092.55c.15.903.932 1.566 1.849 1.566h.344c.916 0 1.699-.663 1.85-1.567l.091-.549a.798.798 0 01.517-.608 7.52 7.52 0 00.478-.198.798.798 0 01.796.064l.453.324a1.875 1.875 0 002.416-.2l.243-.243c.648-.648.733-1.67.2-2.416l-.324-.453a.798.798 0 01-.064-.796c.071-.157.137-.316.198-.478.1-.267.327-.47.608-.517l.55-.091a1.875 1.875 0 001.566-1.85v-.344c0-.916-.663-1.699-1.567-1.85l-.549-.091a.798.798 0 01-.608-.517 7.507 7.507 0 00-.198-.478.798.798 0 01.064-.796l.324-.453a1.875 1.875 0 00-.2-2.416l-.243-.243a1.875 1.875 0 00-2.416-.2l-.453.324a.798.798 0 01-.796.064 7.462 7.462 0 00-.478-.198.798.798 0 01-.517-.608l-.091-.55a1.875 1.875 0 00-1.85-1.566h-.344zM12 15.75a3.75 3.75 0 100-7.5 3.75 3.75 0 000 7.5z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">AT</p>
                </span>
                |
                <span class="flex items-center gap-1"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="h-5 w-5"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"
                      clip-rule="evenodd"
                    />
                  </svg>

                  <p class="">Jakarta Utara</p>
                </span>
              </div>
              <hr class="my-2" />
              <div class="flex items-end justify-between">
                <div class="px-2">
                  <a
                    href="#"
                    class="
                      text-2xl
                      font-bold
                      capitalize
                      text-blue-600
                      transition
                      duration-100
                      hover:text-gray-500
                    "
                  >
                    3.000.000
                    <span class="text-semibold text-xs text-gray-700"
                      >/bulan
                    </span>
                  </a>
                  <p class="text-xs">Uang muka mulai dari Rp. 23.000.000</p>
                </div>
                <button
                  href="#"
                  class="
                    h-10
                    w-10
                    scale-100
                    rounded-full
                    border border-blue-600
                    bg-transparent
                    text-sm
                    font-bold
                    uppercase
                    text-blue-600
                    transition
                    duration-150
                    hover:scale-105
                    hover:bg-blue-700
                    hover:text-yellow-400
                    hover:shadow-lg
                    hover:shadow-blue-700/50
                    focus:z-10
                    focus:outline-none
                    focus:ring-4
                    focus:ring-gray-200
                  "
                >
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    viewBox="0 0 24 24"
                    fill="currentColor"
                    class="mx-auto h-6 w-6"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M3.75 12a.75.75 0 01.75-.75h13.19l-5.47-5.47a.75.75 0 011.06-1.06l6.75 6.75a.75.75 0 010 1.06l-6.75 6.75a.75.75 0 11-1.06-1.06l5.47-5.47H4.5a.75.75 0 01-.75-.75z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
