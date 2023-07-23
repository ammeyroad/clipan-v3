<template>
  <div class="">
    <section
      class="
      carousel
        bg-[url('/background-slider.jpg')] bg-cover bg-no-repeat bg-left
      "
      style="backgroundimage: "
      aria-label="Gallery"
    >
      <ol class="carousel__viewport py-20  bg-[url('/background-slider.jpg')] bg-cover bg-no-repeat bg-left">
        <li id="carousel__slide1" tabindex="0" class="carousel__slide">
          <div class="carousel__snapper"></div>

          <div class="grid sm:grid-cols-2 max-w-screen-lg mx-auto items-center">
            <div class="space-y-8">
              <h3
                class="
                  mb-6
                  font-sans
                  text-4xl
                  font-bold
                  tracking-tight
                  text-white
                  sm:text-5xl sm:leading-none
                "
              >
                PEMBIAYAAN MULTIGUNA UNTUK SEMUA KEBUTUHAN
              </h3>
              <h5 class="hidden sm:flex font-bold text-lg text-left">
                Berawal dari marketplace lalu tumbuh menjadi platform yang
                memberikan banyak kemudahan untuk berbisnis.
              </h5>

              <a
                href="#"
                class="
                  inline-block
                  rounded-lg
                  bg-blue-400
                  px-4
                  py-3
                  text-center text-sm
                  shadow shadow-blue-400/60
                  hover:shadow-blue-400 hover:shadow-lg hover:-translate-y-2
                  font-semibold
                  hover:ring-2 hover:ring-blue-700/50
                  text-white
                  outline-none
                  ring-indigo-300
                  transition
                  duration-100
                  hover:bg-blue-600
                  md:text-base
                  uppercase
                "
              >
                <Icon name="heroicons-outline:hand" class="w-6 h-6 mr-2" />Start
                now</a
              >
            </div>
            <div class="-mt-24 sm:mt-0 p-12">
              <img
                src="/slider-1.png"
                loading="lazy"
                alt="Photo by Fakurian Design"
                class="w-full pt-10"
              />
            </div>
          </div>
        </li>
        <li id="carousel__slide2" tabindex="0" class="carousel__slide">
          <div class="carousel__snapper"></div>
          <div class="flex max-w-screen-lg mx-auto items-center">
            <div class="sm:w-1/2 space-y-8">
              <h3
                class="
                  mb-6
                  font-sans
                  text-4xl
                  font-bold
                  tracking-tight
                  text-white
                  sm:text-5xl sm:leading-none
                "
              >
                PEMBIAYAAN KENDARAAN MOBIL BARU
              </h3>
              <h5 class="hidden sm:flex  font-bold text-lg text-left">
                Berawal dari marketplace lalu tumbuh menjadi platform yang
                memberikan banyak kemudahan untuk berbisnis.
              </h5>

              <a
                href="#"
                class="
                  inline-block
                  rounded-lg
                  bg-blue-400
                  px-4
                  py-3
                  text-center text-sm
                  shadow shadow-blue-400/60
                  hover:shadow-blue-400 hover:shadow-lg hover:-translate-y-2
                  font-semibold
                  hover:ring-2 hover:ring-blue-700/50
                  text-white
                  outline-none
                  ring-indigo-300
                  transition
                  duration-100
                  hover:bg-blue-600
                  md:text-base
                  uppercase
                "
              >
                <Icon name="heroicons-outline:hand" class="w-6 h-6 mr-2" />Start
                now</a
              >
            </div>
            <div class="sm:w-1/2 p-12">
              <img
                src="/slider-2.png"
                loading="lazy"
                alt="Photo by Fakurian Design"
                class="w-full pt-10"
              />
            </div>
          </div>
        </li>
        <li id="carousel__slide3" tabindex="0" class="carousel__slide">
          <div class="carousel__snapper"></div>
          <div class="flex max-w-screen-lg mx-auto items-center">
            <div class="sm:w-1/2 p-12">
              <img
                src="/slider-3.png"
                loading="lazy"
                alt="Photo by Fakurian Design"
                class="w-full"
              />
            </div>

            <div class="sm:w-1/2 space-y-8">
              <h3
                class="
                  mb-6
                  font-sans
                  text-4xl
                  font-bold
                  tracking-tight
                  text-white
                  sm:text-5xl sm:leading-none
                "
              >
                PEMBIAYAAN KENDARAAN MOBIL BARU
              </h3>
              <h5 class="hidden sm:flex  font-bold text-lg text-left">
                Berawal dari marketplace lalu tumbuh menjadi platform yang
                memberikan banyak kemudahan untuk berbisnis.
              </h5>

              <a
                href="#"
                class="
                  inline-block
                  rounded-lg
                  bg-blue-400
                  px-4
                  py-3
                  text-center text-sm
                  shadow shadow-blue-400/60
                  hover:shadow-blue-400 hover:shadow-lg hover:-translate-y-2
                  font-semibold
                  hover:ring-2 hover:ring-blue-700/50
                  text-white
                  outline-none
                  ring-indigo-300
                  transition
                  duration-100
                  hover:bg-blue-600
                  md:text-base
                  uppercase
                "
              >
                <Icon name="heroicons-outline:hand" class="w-6 h-6 mr-2" />Start
                now</a
              >
            </div>
          </div>
        </li>
      </ol>
      <aside class="carousel__navigation">
        <ol class="carousel__navigation-list">
          <li class="carousel__navigation-item">
            <a href="#carousel__slide1" class="carousel__navigation-button"
              >Go to slide 1</a
            >
          </li>
          <li class="carousel__navigation-item">
            <a href="#carousel__slide2" class="carousel__navigation-button"
              >Go to slide 2</a
            >
          </li>
          <li class="carousel__navigation-item">
            <a href="#carousel__slide3" class="carousel__navigation-button"
              >Go to slide 3</a
            >
          </li>
          <li class="carousel__navigation-item">
            <a href="#carousel__slide4" class="carousel__navigation-button"
              >Go to slide 4</a
            >
          </li>
        </ol>
      </aside>
    </section>
      <!-- sejarah singkat -->
  <section class="max-w-screen-lg px-5 mx-auto space-y-12 z-20">
    <div class="">
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
    </div>

    <div class="grid sm:grid-cols-5 sm:space-x-16">
      <div class="sm:col-span-2">
        <img
          src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
          loading="lazy"
          alt="Photo by Fakurian Design"
          class=""
        />
      </div>
      <div class="sm:col-span-3">
        <p class="text-left">
          Berawal dari marketplace lalu tumbuh menjadi platform yang memberikan
          banyak kemudahan untuk berbisnis. Inilah kami, Buka, perusahaan yang
          terus berevolusi dan berinovasi untuk kepentingan bersama.
          <br /><br />

          Dalam tonggak sejarah berikutnya, tepatnya pada 17 Mei 1990, Perseroan
          melakukan perubahan nama dari semula PT Clipan Leasing Corporation
          menjadi PT Clipan Finance Indonesia yang mana perubahan tersebut
          mengacu pada Akta No. 56 tanggal 17 Mei 1990 dan telah disahkan
          melalui Surat Keputusan Menteri Kehakiman Republik Indonesia No.
          C2.3418.HT.01.04.th 90 tanggal 5 Juli 1990.
          <br /><br />

          Dalam rangka memperkuat posisi Perseroan di industri pembiayaan
          nasional, maka pada 27 Agustus 1990 Perseroan resmi melakukan
          penawaran saham perdana di Bursa Efek Jakarta (BEJ) yang kini bernama
          Bursa Efek Indonesia (BEI). Atas aksi korporasi tersebut, Perseroan
          tercatat sebagai perusahaan pembiayaan pertama yang go public di
          Indonesia.
        </p>
      </div>
    </div>

    <div class="flex w-full md:mx-auto md:max-w-screen-xl overflow-x-auto">
      <div class="flex space-x-4">
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
        <div class="w-52 sm:w-1/4 bg-blue-400 p-4">
          <p>sdasdsadsad</p>
          <img
            src="https://images.unsplash.com/photo-1618004912476-29818d81ae2e?auto=format&q=75&fit=crop&w=1000"
            loading="lazy"
            alt="Photo by Fakurian Design"
            class=""
          />
        </div>
      </div>
    </div>
  </section>
  </div>
</template>

<style>
@keyframes tonext {
  75% {
    left: 0;
  }
  95% {
    left: 100%;
  }
  98% {
    left: 100%;
  }
  99% {
    left: 0;
  }
}

@keyframes tostart {
  75% {
    left: 0;
  }
  95% {
    left: -300%;
  }
  98% {
    left: -300%;
  }
  99% {
    left: 0;
  }
}

@keyframes snap {
  96% {
    scroll-snap-align: center;
  }
  97% {
    scroll-snap-align: none;
  }
  99% {
    scroll-snap-align: none;
  }
  100% {
    scroll-snap-align: center;
  }
}

* {
  box-sizing: border-box;
  scrollbar-color: transparent transparent; /* thumb and track color */
  scrollbar-width: 0px;
}

*::-webkit-scrollbar {
  width: 0;
}

*::-webkit-scrollbar-track {
  background: transparent;
}

*::-webkit-scrollbar-thumb {
  background: transparent;
  border: none;
}

* {
  -ms-overflow-style: none;
}

ol,
li {
  list-style: none;
  margin: 0;
  padding: 0;
}

.carousel {
 
  filter: drop-shadow(0 0 10px #0003);
  perspective: 100px;
}

.carousel__viewport {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  display: flex;
  overflow-x: scroll;
  counter-reset: item;
  scroll-behavior: smooth;
  scroll-snap-type: x mandatory;
}

.carousel__slide {
  position: relative;
  flex: 0 0 100%;
  width: 100%;
}

.carousel__slide:before {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate3d(-50%, -40%, 70px);
}

.carousel__snapper {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  scroll-snap-align: center;
}

@media (hover: hover) {
  .carousel__snapper {
    animation-name: tonext, snap;
    animation-timing-function: ease;
    animation-duration: 4s;
    animation-iteration-count: infinite;
  }

  .carousel__slide:last-child .carousel__snapper {
    animation-name: tostart, snap;
  }
}

@media (prefers-reduced-motion: reduce) {
  .carousel__snapper {
    animation-name: none;
  }
}

.carousel:hover .carousel__snapper,
.carousel:focus-within .carousel__snapper {
  animation-name: none;
}

.carousel__navigation {
  position: absolute;
  right: 0;
  bottom: 20px;
  left: 0;
  text-align: center;
}

.carousel__navigation-list,
.carousel__navigation-item {
  display: inline-block;
}

.carousel__navigation-button {
  display: inline-block;
  width: 1.5rem;
  height: 1.5rem;
  background-color: #333;
  background-clip: content-box;
  border: 0.25rem solid transparent;
  border-radius: 50%;
  font-size: 0;
  transition: transform 0.1s;
}
</style>
