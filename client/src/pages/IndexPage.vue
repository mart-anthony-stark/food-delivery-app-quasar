<template>
  <q-page>
    <Navbar />
    <HeaderVue />
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import Navbar from "../components/Navbar.vue";
import HeaderVue from "src/components/index/HeaderSection.vue";

export default defineComponent({
  name: "IndexPage",
  components: { Navbar, HeaderVue },
});
</script>
