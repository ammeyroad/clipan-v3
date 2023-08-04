<template>
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
          <div  v-for="angka in angkas"
            class="
              py-5
              sm:py-12
              text-center
              align-middle
              duration-300
              hover:scale-110 hover:bg-black/5
            "
          >
            <h3 class="px-5 sm:px-12 text-black">
              <b
                ><span class="text-6xl"> {{ angka.angka }} </span><br />
                <p class="text-sm">
                  {{ angka.isi }}
                </p></b
              >
            </h3>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const angkas = [
  {
    angka: '40',
    isi: 'tahun telah berdiri',
  },
  {
    angka: '63',
    isi: 'cabang di indonesia',
  },
  {
    angka: '7T',
    isi: 'total triliun aset',
  },
{
    angka: '3K',
    isi: 'Lebih Karyawan',
  },
]
</script>
