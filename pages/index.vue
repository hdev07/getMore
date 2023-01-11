<template>
  <div>
    <div class="bg-img container">
      <Home id="Home" />
    </div>
    <Accessories />
  </div>
</template>
<script>
import Home from "~~/components/Home.vue";
import Accessories from "~~/components/Accessories.vue";

export default {
  components: { Home, Accessories },
};
</script>
<style lang="scss" scoped>
.container {
  width: 100vw;
  height: 100vh;
}
</style>
