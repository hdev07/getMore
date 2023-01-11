<template>
  <div>
    <Navbar />
    <div class="text-title">
      <p class="Text-Style">
        Las mejores raquetas para jugar
        <span class="Text-Style-6">Tennis</span>
      </p>
      <button class="btn">
        <p>Acerca de nosotros</p>
        <svg
          width="74"
          height="16"
          viewBox="0 0 74 16"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="path-arrow"
        >
          <path
            d="M70.1722 6.778L64.8082 1.414L66.2222 0L74.0002 7.778L66.2222 15.556L64.8082 14.142L70.1722 8.778H0V6.778H70.1722Z"
          />
        </svg>
      </button>
    </div>
  </div>
</template>
<script>
import Navbar from "../components/Navbar.vue";

export default {
  components: { Navbar },
};
</script>
<style lang="scss" scoped>
div .text-title {
  position: absolute;
  width: 40rem;
  top: 100 * $--spacing-xxs;
  left: 43 * $--spacing-xxs;
}
.btn {
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  border: 1px solid #fff;
  background-color: transparent;
  color: #fff;
  width: 269px;
  height: 53px;
  margin-top: 4vh;
  border-radius: 26.5px;
  text-transform: uppercase;
}
.path-arrow {
  fill: #fff;
  width: 1.7rem;
  padding-left: 0.4rem;
}
@media screen and (max-width: 864px) {
  div .text-title {
    position: inherit;
    width: 100vw;
    text-align: center;
    margin: auto;
    padding-top: 30vh;
  }

  div button {
    margin: auto;
  }
}
</style>
