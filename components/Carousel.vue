<template>
  <div class="container-carousel">
    <div class="img-container bg-img">
      <div class="text">
        <p class="Text-Style-2">Nuestras <b>Raquetas</b></p>
        <p class="Text-Style-15">
          Conoce nuestras raquetas y aprende a jugar Tennis cómo un profesional.
        </p>
      </div>
    </div>
    <div class="carousel">
      <div class="carousel-container">
        <div class="carousel-item">
          <img
            class="carousel-item-img"
            src="../assets/images/carousel.png"
            alt="People"
          />
          <div class="carousel-item-details"></div>
        </div>
        <div class="carousel-item">
          <img
            class="carousel-item-img"
            src="../assets/images/carousel.png"
            alt="People"
          />
          <div class="carousel-item-details"></div>
        </div>
        <div class="carousel-item">
          <img
            class="carousel-item-img"
            src="../assets/images/carousel.png"
            alt="People"
          />
          <div class="carousel-item-details"></div>
        </div>
        <div class="carousel-item">
          <img
            class="carousel-item-img"
            src="../assets/images/carousel.png"
            alt="People"
          />
          <div class="carousel-item-details"></div>
        </div>
        <div class="carousel-item">
          <img
            src="../assets/images/carousel.png"
            class="carousel-item-img"
            alt="People"
          />
          <div class="carousel-item-details"></div>
        </div>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.text {
  margin-left: 10vw;
  margin-top: 3vw;
}
.container-carousel > .bg-img {
  background-image: url("../assets/images/ball.png");
  background-repeat: no-repeat;
  background-size: cover;
  width: 35vw;
}
.container-carousel {
  display: flex;
}

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

ol,
li {
  list-style: none;
  margin: 0;
  padding: 0;
}

.carousel {
  width: 65vw;
  overflow: scroll;
  position: relative;
  box-sizing: border-box;
}
.carousel-container {
  white-space: nowrap;
  margin: 70px 20px;
  padding-bottom: 10px;
}
.carousel-item {
  width: 200px;
  height: 250px;
  border-radius: 20px;
  overflow: hidden;
  margin-right: 10px;
  display: inline-block;
  cursor: pointer;
  transition: 450ms all;
  transform-origin: center left;
  position: relative;
}
.carousel-item:hover ~ .carousel-item {
  transform: translate3d(100px, 0, 0);
}
.carousel-container:hover .carousel-item {
  opacity: 0.4;
}
.carousel-container:hover .carousel-item:hover {
  transform: scale(1.5);
  opacity: 1;
}
.carousel-item-img {
  width: 200px;
  height: 250px;
  object-fit: cover;
}
.carousel::-webkit-scrollbar {
  height: 0px;
}

.carousel::-webkit-scrollbar-track {
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}
.carousel::-webkit-scrollbar-track-piece {
  max-width: 100px;
}
.carousel::-webkit-scrollbar-thumb {
  border-radius: 10px;
  box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.5);
  background-color: gray;
}
</style>
