<template>
 <div class="px-2 bg-blue-500">
  <section class="carousel" aria-label="Gallery">
    <ol class="carousel__viewport h-full">
      <li id="carousel__slide1" tabindex="0" class="carousel__slide">
        <div class="carousel__snapper"></div>
        sdsadsd slide1
        <p class="head2">slediea</p>
      </li>
      <li id="carousel__slide2" tabindex="0" class="carousel__slide">
        sdsadsd slide2
        <p class="head2">slediea</p>
        <div class="carousel__snapper"></div>
      </li>
      <li id="carousel__slide3" tabindex="0" class="carousel__slide">
        <div class="carousel__snapper"></div>
        sdsadsd slide3
        <p class="head2">slediea</p>
      </li>
      <li id="carousel__slide4" tabindex="0" class="carousel__slide">
        <div class="carousel__snapper"></div>
        sdsadsd slide4
        <p class="head2">slediea</p>
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
  padding-top: 5%;
  filter: drop-shadow(0 0 10px #0003);
  height: 600px;
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
    height: 600px;
  background-color: #f99;
  counter-increment: item;
}

.carousel__slide:nth-child(even) {
  background-color: #99f;
  
}


.carousel:hover .carousel__snapper,
.carousel:focus-within .carousel__snapper {
  animation-name: none;
}

.carousel__navigation {
  position: absolute;
  right: 0;
  bottom: 25px;
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
