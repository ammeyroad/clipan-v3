<template>
  <div class="">
    <section
      class="
        carousel
        h-[700px]
        bg-[url('/background-slider.jpg')] bg-cover bg-no-repeat bg-left
      "
      style="backgroundimage: "
      aria-label="Gallery"
    >
      <ol class="carousel__viewport h-full">
        <li id="carousel__slide1" tabindex="0" class="carousel__slide p-5">
          <div class="carousel__snapper"></div>

          <div class="grid sm:grid-cols-2 max-w-screen-lg mx-auto items-center mt-20">
            <div class=" space-y-8">
              <h3 class="mb-6 font-sans text-4xl font-bold tracking-tight text-white sm:text-5xl sm:leading-none">
                PEMBIAYAAN MULTIGUNA UNTUK SEMUA KEBUTUHAN
              </h3>
              <h5 class="font-bold text-lg text-left">
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
          <div class="flex max-w-screen-lg mx-auto items-center mt-20">
            <div class="sm:w-1/2 space-y-8">
              <h3 class="mb-6 font-sans text-4xl font-bold tracking-tight text-white sm:text-5xl sm:leading-none">
                PEMBIAYAAN KENDARAAN MOBIL BARU
              </h3>
              <h5 class="font-bold text-lg text-left">
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
          <div class="flex max-w-screen-lg mx-auto items-center mt-20">
            <div class="sm:w-1/2 p-12">
              <img
                src="/slider-3.png"
                loading="lazy"
                alt="Photo by Fakurian Design"
                class="w-full"
              />
            </div>

            <div class="sm:w-1/2 space-y-8">
              <h3 class="mb-6 font-sans text-4xl font-bold tracking-tight text-white sm:text-5xl sm:leading-none">
                PEMBIAYAAN KENDARAAN MOBIL BARU
              </h3>
              <h5 class="font-bold text-lg text-left">
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
  position: relative;
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
