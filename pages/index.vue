<template>
  <div>
    <div class="bg-img container">
      <Home id="Home" />
    </div>
    <Accessories />
    <Carousel />
    <Banner />
    <Footer />
  </div>
</template>
<script>
import Home from "~~/components/Home.vue";
import Accessories from "~~/components/Accessories.vue";
import Carousel from "~~/components/Carousel.vue";
import Banner from "~~/components/Banner.vue";
import Footer from "~~/components/Footer.vue";

export default {
  components: { Home, Accessories, Carousel, Banner, Footer },
};
</script>
<style lang="scss" scoped>
.container {
  width: 100vw;
  height: 100vh;
}
</style>
