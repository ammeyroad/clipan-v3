<template>
  <div class="">
    <section class="carousel">
      <ol
        class="
          carousel__viewport
          bg-center
          h-full
          bg-[url('/background-slider.jpg')] bg-cover bg-no-repeat bg-left
          pb-14
        "
      >
        <li id="carousel__slide1" tabindex="0" class="carousel__slide py-12">
          <div class="carousel__snapper"></div>

          <div
            class="
              flex-col
              sm:flex-row-reverse
              flex
              max-w-screen-xl
              mx-auto
              items-center
              p-5
            "
          >
            <div class="sm:w-1/2 sm:p-5">
              <img
                src="/slider-1.png"
                loading="lazy"
                alt="Photo by Fakurian Design"
                class="px-12 sm:p-4"
              />
            </div>
            <div class="sm:w-1/2">
              <h3
                class="
                  mb-6
                  font-sans
                  text-2xl
                  leading-none
                  text-white text-center
                  sm:text-left sm:text-5xl sm:leading-none
                  uppercase
                  drop-shadow-lg
                  drop-shadow-blue
                "
              >
                Pengajuannya gampang, bunganya buat senang
              </h3>
              <h5 class="hidden sm:flex font-bold text-left sm:mb-5 text-white">
                Berawal dari marketplace lalu tumbuh menjadi platform yang
                memberikan banyak kemudahan untuk berbisnis.
              </h5>
              <div class="px-24 sm:px-0">
                <button
                  type="button"
                  class="
                   btn-w
                  "
                >
                  Selengkapnya
                </button>
              </div>
            </div>
          </div>
        </li>
        <li id="carousel__slide2" tabindex="0" class="carousel__slide py-12">
          <div class="carousel__snapper"></div>
          <div
            class="
              flex-col
              sm:flex-row-reverse
              flex
              max-w-screen-xl
              mx-auto
              items-center
              p-5
            "
          >
            <div class="sm:w-1/2 sm:p-5">
              <img
                src="/slider-2.png"
                loading="lazy"
                alt="Photo by Fakurian Design"
                class="px-12 sm:p-4"
              />
            </div>
            <div class="sm:w-1/2">
              <h3
                class="
                  mb-6
                  font-sans
                  text-2xl
                  font-extrabold
                  leading-none
                  text-white text-center
                  sm:text-left sm:text-5xl sm:leading-none
                  uppercase
                "
              >
                Bunga spesial 0% khusus pengajuan bulan ini
              </h3>
              <h5 class="hidden sm:flex font-bold text-left sm:mb-5 text-white">
                Berawal dari marketplace lalu tumbuh menjadi platform yang
                memberikan banyak kemudahan untuk berbisnis.
              </h5>
              <div class="px-24 sm:px-0">
                <button
                  type="button"
                  class="
                    w-full
                    sm:w-max
                    text-blue-600
                    font-bold
                    bg-white
                    hover:bg-gray-200
                    focus:ring-4 focus:ring-blue-300
                    rounded-lg
                    text-sm
                    uppercase
                    py-3.5
                    px-4
                  "
                >
                  Selengkapnya
                </button>
              </div>
            </div>
          </div>
        </li>
        <li id="carousel__slide3" tabindex="0" class="carousel__slide py-12">
          <div class="carousel__snapper"></div>
          <div
            class="
              flex-col
              sm:flex-row-reverse
              flex
              max-w-screen-xl
              mx-auto
              items-center
              p-5
            "
          >
            <div class="sm:w-1/2 sm:p-5">
              <img
                src="/slider-3.png"
                loading="lazy"
                alt="Photo by Fakurian Design"
                class="px-12 sm:p-4"
              />
            </div>
            <div class="sm:w-1/2">
              <h3
                class="
                  mb-6
                  font-sans
                  text-2xl
                  font-extrabold
                  leading-none
                  text-white text-center
                  sm:text-left sm:text-5xl sm:leading-none
                  uppercase
                "
              >
                Aman berkendara dengan fitur roadman assistant
              </h3>
              <h5 class="hidden sm:flex font-bold text-left sm:mb-5 text-white">
                Berawal dari marketplace lalu tumbuh menjadi platform yang
                memberikan banyak kemudahan untuk berbisnis.
              </h5>
              <div class="px-24 sm:px-0">
                <button
                  type="button"
                  class="
                    w-full
                    sm:w-max
                    text-blue-600
                    font-bold
                    bg-white
                    hover:bg-gray-200
                    focus:ring-4 focus:ring-blue-300
                    rounded-lg
                    text-sm
                    uppercase
                    py-3.5
                    px-4
                  "
                >
                  Selengkapnya
                </button>
              </div>
            </div>
          </div>
        </li>
      </ol>
      <aside class="carousel__navigation">
        <ol class="carousel__navigation-list">
          <li class="carousel__navigation-item">
            <a
              href="#carousel__slide1"
              class="
                carousel__navigation-button
                hover:opacity-100
                bg-white
                opacity-50
              "
              >Go to slide 1</a
            >
          </li>
          <li class="carousel__navigation-item">
            <a
              href="#carousel__slide2"
              class="
                carousel__navigation-button
                hover:opacity-100
                bg-white
                opacity-50
              "
              >Go to slide 2</a
            >
          </li>
          <li class="carousel__navigation-item">
            <a
              href="#carousel__slide3"
              class="
                carousel__navigation-button
                hover:opacity-100
                bg-white
                opacity-50
              "
              >Go to slide 3</a
            >
          </li>
        </ol>
      </aside>
    
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
  bottom: 17%;
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
  background-clip: content-box;
  border: 0.25rem solid transparent;
  border-radius: 50%;
  font-size: 0;
  transition: transform 0.1s;
}
</style>
