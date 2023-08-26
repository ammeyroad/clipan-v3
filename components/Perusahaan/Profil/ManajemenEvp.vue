<template>
  <div class="flex py-12 w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
    <div class="flex sm:flex-wrap">
      <div v-for="daftar in rups" class="px-4 w-72 sm:w-1/3">
        <div
          class="
            rounded-xl
            hover:shadow-lg
            bg-white
            hover:bg-gray-50
            rounded-xl
            duration-200
          "
        >
          <div class="">
            <h4
              class="
                uppercase
                text-white
                rounded-t-xl
                bg-blue-600
                text-2xl
                font-bold
                text-center
                p-4
              "
            >
              Tahun {{ daftar.tahun }}
            </h4>
          </div>
          <ul class="divide-y divide-gray-300/50 p-2">
            <li
              v-for="link in daftar.daftars"
              class="
                flex
                items-center
                px-4
                py-4
                justify-between
                group
                hover:bg-white hover:shadow-md
                rounded-lg
                duration-200
              "
            >
              <p
                class="
                  group-hover:font-bold group-hover:text-blue-600
                  duration-200
                  capitalize
                "
              >
                {{ link.judul }}
              </p>

              <div class="flex">
                <a
                  v-for="file in link.download"
                  :href="file.to"
                  class="
                    opacity-50
                    group-hover:opacity-100
                    scale-75
                    fill-gray-400
                    group-hover:scale-100
                    duration-200
                    hover:animate-bounce hover:fill-blue-600
                  "
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    width="32"
                    height="32"
                    viewBox="0 0 24 24"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M2 12c0-4.714 0-7.071 1.464-8.536C4.93 2 7.286 2 12 2c4.714 0 7.071 0 8.535 1.464C22 4.93 22 7.286 22 12c0 4.714 0 7.071-1.465 8.535C19.072 22 16.714 22 12 22s-7.071 0-8.536-1.465C2 19.072 2 16.714 2 12Zm10-5.75a.75.75 0 0 1 .75.75v5.19l1.72-1.72a.75.75 0 1 1 1.06 1.06l-3 3a.75.75 0 0 1-1.06 0l-3-3a.75.75 0 1 1 1.06-1.06l1.72 1.72V7a.75.75 0 0 1 .75-.75Zm-4 10a.75.75 0 0 0 0 1.5h8a.75.75 0 0 0 0-1.5H8Z"
                      clip-rule="evenodd"
                    />
                  </svg>
                </a>
              </div>
            </li>
          </ul>
        </div>
      </div>

      <div class="w-72">a</div>
    </div>
  </div>
</template>
<script setup>
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue';
const rups = [
  {
    tahun: '2023',
    daftars: [
      {
        judul: 'Pengumuman',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Pemanggilan',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Surat Kuasa',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Tata Tertib',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Informasi Dividen',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
    ],
  },
  {
    tahun: '2022',
    daftars: [
      {
        judul: 'Pengumuman',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Pemanggilan',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Surat Kuasa',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Tata Tertib',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Informasi Dividen',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
    ],
  },
  {
    tahun: '2022',
    daftars: [
      {
        judul: 'Pengumuman',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Pemanggilan',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Surat Kuasa',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Tata Tertib',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Informasi Dividen',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
    ],
  },
  {
    tahun: '2022',
    daftars: [
      {
        judul: 'Pengumuman',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Pemanggilan',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Surat Kuasa',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Tata Tertib',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
      {
        judul: 'Informasi Dividen',
        download: [
          {
            to: '/profile#tentang',
          },
          {
            to: '/prof',
          },
        ],
      },
    ],
  },
];
</script>
