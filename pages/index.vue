<template>
  <div class="bg-img container">
    <Home />
  </div>
</template>
<script>
import Home from "~~/components/Home.vue";

export default {
  components: { Home },
};
</script>
<style lang="scss" scoped>
.container {
  width: 100vw;
  height: 100vh;
}
</style>
