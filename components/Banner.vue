<template>
  <div class="bg-img"></div>
</template>

<style lang="scss" scoped>
div {
  height: 50vh;
}
.bg-img {
  background-image: url("../assets/images/banner.png");
  background-repeat: no-repeat;
  background-size: cover;
}

@media screen and (max-width: 864px) {
  .bg-img {
    background-position: 7%;
  }
}
</style>
