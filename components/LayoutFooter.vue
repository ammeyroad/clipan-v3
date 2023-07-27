<template>
  <Footer class="pt-12 lg:pt-16 bg-blue-600 text-white mb-16 sm:mb-0">
    <div class="mx-auto max-w-screen-xl">
      <div class="mx-auto max-w-screen-2xl px-4 md:px-8">
        <div class="mb-16 grid grid-cols-2 gap-2 md:grid-cols-5 lg:gap-4">
          <div class="p-2 col-span-2">
            <!-- logo - start -->
            <div class="mb-2 lg:-mt-2">
              <a href="/">
                <img
                  src="https://clipan.co.id/wp-content/uploads/2021/07/LOGO-CLIPAN-FINAL-1536x206.png"
                  class="w-1/2"
                  alt=""
              /></a>
            </div>
            <!-- logo - end -->

            <p class="mb-5 sm:pr-8">
              <b>PT Clipan Finance Indonesia</b> <br />
              Perusahaan pembiayaan untuk mobil baru, mobil bekas, alat berat,
              dan multiguna.
            </p>

            <!-- social - start -->
            <div class="flex">
              <a v-for="item in soc" :href="item.to" class="mr-1 rounded-lg">
                <div v-html="item.icon" class="w-10 h-10"></div>
              </a>
              <select
                id="countries"
                class="
                  bg-black/10
                  border border-blue-600
                  text-white text-sm
                  rounded-lg
                  w-max
                  block
                "
              >
                <option>Bahasa</option>
                <option>English</option>
              </select>
            </div>
            <!-- social - end -->
          </div>

          <a
            v-for="item in fot"
            :href="item.to"
            class="p-5 hover:bg-black/20 rounded-xl duration-300"
          >
            <div class="bg-black/10 p-3 rounded-lg w-12 h-12 mb-2">
              <div v-html="item.icon" class="w-6 h-6 mr-2"></div>
              <div></div>
            </div>
            <p class="font-black text-white text-lg lowercase">
              {{ item.isi }}
            </p>
            <p class="font-semibold text-white tracking-tighter mt-4">
              {{ item.judul }}
            </p>
            <p class="mx-auto text-xs">{{ item.ket }}</p>
          </a>
        </div>

        <div
          class="
            bg-black/20
            rounded-t-lg
            py-4
            justify-beetwen
            mx-auto
            w-full
            text-sm
            flex
          "
        >
          <p class="text-center mx-auto">
            <svg
              class="w-4 fill-white inline"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g id="SVGRepo_bgCarrier" stroke-width="0"></g>
              <g
                id="SVGRepo_tracerCarrier"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></g>
              <g id="SVGRepo_iconCarrier">
                <path
                  opacity="0.5"
                  d="M3.37752 5.08241C3 5.62028 3 7.21907 3 10.4167V11.9914C3 17.6294 7.23896 20.3655 9.89856 21.5273C10.62 21.8424 10.9807 22 12 22C13.0193 22 13.38 21.8424 14.1014 21.5273C16.761 20.3655 21 17.6294 21 11.9914V10.4167C21 7.21907 21 5.62028 20.6225 5.08241C20.245 4.54454 18.7417 4.02996 15.7351 3.00079L15.1623 2.80472C13.595 2.26824 12.8114 2 12 2C11.1886 2 10.405 2.26824 8.83772 2.80472L8.26491 3.00079C5.25832 4.02996 3.75503 4.54454 3.37752 5.08241Z"
                  fill="#ffffff"
                ></path>
                <path
                  d="M15.0595 10.4995C15.3353 10.1905 15.3085 9.71643 14.9995 9.44055C14.6905 9.16468 14.2164 9.19152 13.9406 9.5005L10.9286 12.8739L10.0595 11.9005C9.78359 11.5915 9.30947 11.5647 9.0005 11.8406C8.69152 12.1164 8.66468 12.5905 8.94055 12.8995L10.3691 14.4995C10.5114 14.6589 10.7149 14.75 10.9286 14.75C11.1422 14.75 11.3457 14.6589 11.488 14.4995L15.0595 10.4995Z"
                  fill="#ffffff"
                ></path>
              </g>
            </svg>
            Clipan finance terdaftar dan diawasi oleh OJK | © 2023 -
            clipanfinance
          </p>
        </div>
      </div>
    </div>
  </Footer>
</template>

<script setup>
const fot = [
  {
    judul: 'Telepon',
    isi: '1500 333',
    to: 'tel:+62215308005',
    ket: 'Senin – Jumat, 08.30-16.00',
    icon: `<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M21 10H14.6C14.0399 10 13.7599 10 13.546 9.89101C13.3578 9.79513 13.2049 9.64215 13.109 9.45399C13 9.24008 13 8.96005 13 8.4V5M10 5H17.8C18.9201 5 19.4802 5 19.908 5.21799C20.2843 5.40973 20.5903 5.71569 20.782 6.09202C21 6.51984 21 7.07989 21 8.2V17.8C21 18.9201 21 19.4802 20.782 19.908C20.5903 20.2843 20.2843 20.5903 19.908 20.782C19.4802 21 18.9201 21 17.8 21H6.2C5.07989 21 4.51984 21 4.09202 20.782C3.71569 20.5903 3.40973 20.2843 3.21799 19.908C3 19.4802 3 18.9201 3 17.8V8.2C3 7.07989 3 6.51984 3.21799 6.09202C3.40973 5.71569 3.71569 5.40973 4.09202 5.21799C4.49359 5.01338 5.01165 5.00082 6 5.00005M10 5V4.6C10 4.03995 10 3.75992 9.89101 3.54601C9.79513 3.35785 9.64215 3.20487 9.45399 3.10899C9.24008 3 8.96005 3 8.4 3H7.6C7.03995 3 6.75992 3 6.54601 3.10899C6.35785 3.20487 6.20487 3.35785 6.10899 3.54601C6 3.75992 6 4.03995 6 4.6V5.00005M10 5V15.4C10 15.9601 10 16.2401 9.89101 16.454C9.79513 16.6422 9.64215 16.7951 9.45399 16.891C9.24008 17 8.96005 17 8.4 17H7.6C7.03995 17 6.75992 17 6.54601 16.891C6.35785 16.7951 6.20487 16.6422 6.10899 16.454C6 16.2401 6 15.9601 6 15.4V5.00005M14 14H14.01V13.99H14V14ZM14 17H14.01V17.01H14V17ZM17 17H17.01V17.01H17V17ZM17 14H17.01V14.01H17V14Z" stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path> </g></svg>`,
  },
  {
    judul: 'Lokasi Cabang',
    isi: 'Jam Layanan',
    to: '/cabang',
    ket: 'Senin – Jumat, 08.30-16.00',
    icon: `<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M6 7H7M6 10H7M11 10H12M11 13H12M6 13H7M11 7H12M11 21V18C11 16.8954 10.1046 16 9 16C7.89543 16 7 16.8954 7 18V21M11 21H12.5M11 21H7M7 21H3V4.6C3 4.03995 3 3.75992 3.10899 3.54601C3.20487 3.35785 3.35785 3.20487 3.54601 3.10899C3.75992 3 4.03995 3 4.6 3H13.4C13.9601 3 14.2401 3 14.454 3.10899C14.6422 3.20487 14.7951 3.35785 14.891 3.54601C15 3.75992 15 4.03995 15 4.6V12M20.8832 16.0318C20.8207 16.0353 20.7578 16.0371 20.6944 16.0371C19.7553 16.0371 18.8987 15.6449 18.25 15C17.6013 15.6449 16.7446 16.0371 15.8056 16.0371C15.7422 16.0371 15.6793 16.0353 15.6168 16.0318C15.5405 16.3588 15.5 16.7018 15.5 17.0554C15.5 18.9532 16.6685 20.5479 18.25 21C19.8315 20.5479 21 18.9532 21 17.0554C21 16.7019 20.9595 16.3589 20.8832 16.0318Z" stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path> </g></svg>`,
  },
    {
    judul: 'Email',
    isi: 'cs@clipan.co.id',
    to: 'mailto:cs@clipan.co.id',
    ket: 'Senin – Jumat, 08.30-16.00',
    icon: `<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M14.5 9.50012H9.5M3.02832 10.0001L10.2246 14.8167C10.8661 15.2444 11.1869 15.4582 11.5336 15.5413C11.8399 15.6147 12.1593 15.6147 12.4657 15.5413C12.8124 15.4582 13.1332 15.2444 13.7747 14.8167L20.971 10.0001M10.2981 4.06892L4.49814 7.71139C3.95121 8.05487 3.67775 8.2266 3.4794 8.45876C3.30385 8.66424 3.17176 8.90317 3.09111 9.16112C3 9.45256 3 9.77548 3 10.4213V16.8001C3 17.9202 3 18.4803 3.21799 18.9081C3.40973 19.2844 3.71569 19.5904 4.09202 19.7821C4.51984 20.0001 5.0799 20.0001 6.2 20.0001H17.8C18.9201 20.0001 19.4802 20.0001 19.908 19.7821C20.2843 19.5904 20.5903 19.2844 20.782 18.9081C21 18.4803 21 17.9202 21 16.8001V10.4213C21 9.77548 21 9.45256 20.9089 9.16112C20.8282 8.90317 20.6962 8.66424 20.5206 8.45876C20.3223 8.2266 20.0488 8.05487 19.5019 7.71139L13.7019 4.06891C13.0846 3.68129 12.776 3.48747 12.4449 3.41192C12.152 3.34512 11.848 3.34512 11.5551 3.41192C11.224 3.48747 10.9154 3.68129 10.2981 4.06892Z" stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path> </g></svg>`,
  },
];

const soc = [
  {
    icon: `<svg class="fill-white hover:fill-yellow-600" viewBox="0 0 32 32" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <title></title> <g id="Instagram"> <path d="M26.49,30H5.5A3.35,3.35,0,0,1,3,29a3.35,3.35,0,0,1-1-2.48V5.5A3.35,3.35,0,0,1,3,3,3.35,3.35,0,0,1,5.5,2h21A3.35,3.35,0,0,1,29,3,3.35,3.35,0,0,1,30,5.5v21A3.52,3.52,0,0,1,26.49,30ZM24.74,10.56a3.45,3.45,0,0,0-3.48-3.49H10.71a3.47,3.47,0,0,0-3.48,3.49V21.1a3.45,3.45,0,0,0,3.48,3.49H21.26a3.43,3.43,0,0,0,3.48-3.49Zm-8.73.9a4.09,4.09,0,0,0-1.38.24,5.36,5.36,0,0,0-1.24.63H9v-.87a2.56,2.56,0,0,1,2.61-2.62h8.75a2.63,2.63,0,0,1,1.89.75A2.48,2.48,0,0,1,23,11.46v.87H18.6a6.14,6.14,0,0,0-1.22-.63A3.87,3.87,0,0,0,16,11.46Zm4.35,11.41H11.61a2.48,2.48,0,0,1-1.86-.78A2.57,2.57,0,0,1,9,20.24v-7h3.49a5.49,5.49,0,0,0-.63,1.23,3.82,3.82,0,0,0-.25,1.4A4.19,4.19,0,0,0,12,17.55a5,5,0,0,0,.93,1.39,4.28,4.28,0,0,0,1.4.95,4.24,4.24,0,0,0,1.72.35,4.29,4.29,0,0,0,3.08-1.3A5,5,0,0,0,20,17.55a4.19,4.19,0,0,0,.35-1.69,3.82,3.82,0,0,0-.25-1.4,6.37,6.37,0,0,0-.6-1.23H23v7a2.52,2.52,0,0,1-.78,1.85A2.57,2.57,0,0,1,20.36,22.87ZM16,13.23a2.55,2.55,0,0,1,1.85.75,2.63,2.63,0,0,1,0,3.74,2.55,2.55,0,0,1-1.85.75,2.63,2.63,0,0,1-1.9-.75,2.66,2.66,0,0,1,0-3.74A2.63,2.63,0,0,1,16,13.23Zm3.5-1.77h1.75V9.71H19.51Z"></path> </g> </g></svg>`,
    to: 'https://www.instagram.com/clipan_official/',
  },
  {
    icon: `<svg class="fill-white hover:fill-yellow-600" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 24 24" xml:space="preserve"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <style type="text/css"> .st0{fill:none;} </style> <path d="M20,2H4C2.9,2,2,2.9,2,4v16c0,1.1,0.9,2,2,2h16c1.1,0,2-0.9,2-2V4C22,2.9,21.1,2,20,2z M18.4,7.4H17c-0.9,0-1,0.3-1,1v1.3 h2.1L18,12h-1.9v7h-3.2v-7h-1.2V9.6h1.2V8.1c0-2,0.8-3.1,3.1-3.1h2.4V7.4z"></path> <rect class="st0" width="24" height="24"></rect> </g></svg>`,
    to: 'https://www.facebook.com/clipan.official/',
  },
  {
    icon: `<svg class="fill-white hover:fill-yellow-600" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 24 24" xml:space="preserve"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <style type="text/css"> .st0{fill:none;} </style> <path d="M20,2H4C2.9,2,2,2.9,2,4v16c0,1.1,0.9,2,2,2h16c1.1,0,2-0.9,2-2V4C22,2.9,21.1,2,20,2z M17.6,8.8c0,0.1,0,0.2,0,0.4 c0,3.8-2.9,8.2-8.2,8.2c-1.6,0-3.1-0.5-4.4-1.3c0.2,0,0.5,0,0.7,0c1.3,0,2.6-0.5,3.6-1.2c-1.3,0-2.3-0.9-2.7-2C6.8,12.9,7,13,7.1,13 c0.3,0,0.5,0,0.8-0.1c-1.3-0.3-2.3-1.4-2.3-2.8l0,0c0.4,0.2,0.8,0.3,1.3,0.4C6.1,9.8,5.6,9,5.6,8c0-0.5,0.1-1,0.4-1.4 c1.4,1.7,3.5,2.9,5.9,3c0-0.2-0.1-0.4-0.1-0.7c0-1.6,1.3-2.9,2.9-2.9c0.8,0,1.6,0.3,2.1,0.9c0.7-0.1,1.3-0.4,1.8-0.7 c-0.2,0.7-0.7,1.2-1.3,1.6c0.6-0.1,1.1-0.2,1.7-0.5C18.6,7.9,18.1,8.4,17.6,8.8z"></path> <rect class="st0" width="24" height="24"></rect> </g></svg>`,
    to: 'https://twitter.com/clipan_official',
  },
  {
    icon: `<svg class="fill-white hover:fill-yellow-600" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 24 24" xml:space="preserve"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <style type="text/css"> .st0{fill:none;} </style> <path d="M20,2H4C2.9,2,2,2.9,2,4v16c0,1.1,0.9,2,2,2h16c1.1,0,2-0.9,2-2V4C22,2.9,21.1,2,20,2z M8.1,18H5V9.4h3.1V18z M6.5,8.4 L6.5,8.4C5.6,8.4,5,7.8,5,7s0.6-1.4,1.6-1.4c0.9,0,1.5,0.6,1.5,1.4S7.5,8.4,6.5,8.4z M19,18h-3.1v-4.7c0-1.3-0.8-1.6-1.1-1.6 s-1.3,0.2-1.3,1.6c0,0.2,0,4.7,0,4.7h-3.1V9.4h3.1v1.2c0.4-0.7,1.2-1.2,2.7-1.2s2.7,1.2,2.7,3.9L19,18L19,18z"></path> <rect class="st0" width="24" height="24"></rect> </g></svg>`,
    to: 'https://www.linkedin.com/company/pt-clipan-finance-indonesia-tbk',
  },
];
</script>
