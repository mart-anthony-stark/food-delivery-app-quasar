<template>
  <q-page class="page">
    <Navbar />
    <HeaderVue />
    <TodaysTrending />
    <PopularItems />
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import Navbar from "../components/Navbar.vue";
import HeaderVue from "src/components/index/HeaderSection.vue";
import TodaysTrending from "src/components/trending/TodaysTrending.vue";
import PopularItems from "src/components/popular/PopularItems.vue";

export default defineComponent({
  name: "IndexPage",
  components: { Navbar, HeaderVue, TodaysTrending, PopularItems },
});
</script>

<style scoped>
.page {
  background: rgb(255, 255, 240);
  background: linear-gradient(
    153deg,
    rgba(255, 255, 240, 1) 0%,
    rgba(244, 236, 225, 1) 61%,
    rgba(244, 236, 225, 1) 100%
  );
}
</style>
