<template>
  <div>
            <div class="bg-gray-100 rounded-t-lg p-2 pb-2 sm:px-10">
              <div class="text-center mb-2">
                <h3 class="mb-4 font-bold text-blue-600 text-lg">
                  Simulasi Kredit
                </h3>
              </div>
              <div class="grid grid-cols-3 content-center">
                <p class="font-bold text-sm">Tenor</p>
                <p class="font-bold text-center text-sm">Total DP</p>
                <p class="font-bold text-right text-sm">Angsuran</p>
              </div>
            </div>
            <div class="p-2 sm:p-4">
              <div
                v-for="n in 5"
                class="
                  grid grid-cols-3
                  content-center
                  py-4
                  px-2
                  hover:font-bold
                  rounded-lg
                  border-b
                  hover:text-blue-600 hover:bg-gray-100
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
                <div for="contact-form-consent-input" class="text-sm">
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
                Ajukan Sekarang
              </button>
            </div>
           </div>
           </template>