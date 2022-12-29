<template>
  <q-page>
    <Navbar />
    <HeaderVue />
    <TodaysTrending />
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import Navbar from "../components/Navbar.vue";
import HeaderVue from "src/components/index/HeaderSection.vue";
import TodaysTrending from "src/components/trending/TodaysTrending.vue";

export default defineComponent({
  name: "IndexPage",
  components: { Navbar, HeaderVue, TodaysTrending },
});
</script>
