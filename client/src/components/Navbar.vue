<template>
  <q-header
    class="row bg-white text-black flex justify-between items-center q-pa-lg"
    reveal
  >
    <!-- Logo -->
    <div class="row">
      <img
        src="~assets/main/logo.svg"
        alt="Foo logo"
        class="q-pr-sm"
        fit="contain"
      />
      <div class="text-h6">Foo</div>
    </div>

    <!-- Nav links -->
    <div class="links col flex justify-center items-center">
      <router-link
        v-for="link in links"
        :key="link.text"
        :to="link.url"
        class="q-px-md text-black text-h6"
        >{{ link.text }}</router-link
      >
    </div>

    <!-- Search -->
    <div class="flex items-center">
      <q-input
        rounded
        standout="bg-primary text-white"
        input-style="width:200px;"
        v-model="text"
        label="Search"
        class="q-mr-md"
      >
        <template v-slot:prepend><q-icon name="search" /></template>
        <template v-slot:append>
          <div class="relative-position">
            <q-icon size="md" name="shopping_cart" color="black-100"> </q-icon>
            <q-badge rounded color="red" floating>2</q-badge>
          </div>
        </template>
      </q-input>
    </div>
  </q-header>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainHeader",
  data() {
    return {
      links: [
        { text: "Home", url: "" },
        { text: "Menu", url: "/menu" },
        { text: "Shop", url: "/shop" },
        { text: "Contact", url: "/contact" },
      ],
    };
  },
});
</script>

<style scoped>
a:-webkit-any-link {
  text-decoration: none !important;
}
</style>
