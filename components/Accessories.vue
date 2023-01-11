<template>
  <div class="container-desc">
    <div class="text-description">
      <div class="p1">
        <p class="Text-Style-12 hidden">Tennis</p>
      </div>
      <div class="p2">
        <p class="Text-Style-4">Raquetas. Accesorios. Pelotas.</p>
        <p class="Text-Style-3 text-gray">
          Conoce nuestras raquetas y aprende a jugar Tennis cómo un profesional.
        </p>
      </div>
      <div class="container-btn">
        <button class="btn">
          <p>Historia</p>
          <svg
            width="74"
            height="16"
            viewBox="0 0 74 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="path"
          >
            <path
              d="M70.1722 6.778L64.8082 1.414L66.2222 0L74.0002 7.778L66.2222 15.556L64.8082 14.142L70.1722 8.778H0V6.778H70.1722Z"
            />
          </svg>
        </button>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.container-desc {
  width: 100vw;
  height: 26.5rem;
  display: flex;
  justify-content: center;
  background-color: #f3f4f8;
  padding-top: 24 * $--spacing-xxs;
}

.container-desc .text-description {
  display: flex;
}

.container-desc .text-description .p1 {
  text-align: end;
  padding-right: 4rem;
}

.container-desc .text-description .p2 {
  width: 38vw;
}

.container-desc .text-gray {
  padding-top: 3rem;
  width: 30vw;
}

.container-desc .text-description .container-btn .btn {
  display: flex;
  justify-content: space-around;
  align-items: center;
  cursor: pointer;
  border: 1px solid #282e47;
  background-color: transparent;
  color: #282e47;
  width: 234px;
  height: 53px;
  border-radius: 26.5px;
  text-transform: uppercase;
}

.container-desc .text-description .container-btn .path {
  fill: #282e47;
  width: 1.7rem;
  padding-left: 0.4rem;
}

.container-desc .text-description .container-btn {
  margin-top: 17%;
  margin-left: 6%;
}
@media screen and (max-width: 864px) {
  .container-desc {
    padding-top: 3rem;
    height: 40%;
  }
  .container-desc div {
    flex-direction: column;
  }
  .container-desc .text-description .p1 {
    display: flex;
    width: 100vw;
    text-align: center;
  }
  .container-desc .text-description .p2 {
    text-align: center;
    display: flex;
    width: 100vw;
  }
  .container-desc .text-gray {
    display: flex;
    width: 100vw;
    margin-bottom: 3rem;
  }
  .container-desc .text-description .container-btn {
    margin: auto;
    display: flex;
    text-align: center;
    justify-content: center;
    padding-bottom: 3vh;
  }
  .hidden {
    display: none;
  }
}
</style>
