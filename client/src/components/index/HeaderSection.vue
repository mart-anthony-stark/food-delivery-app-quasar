<template>
  <section class="row flex justify-center">
    <div class="col column items-start q-gutter-lg" style="max-width: 500px">
      <q-img
        fit="contain"
        src="~assets/main/tagline.svg"
        style="width: 400px"
      />

      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus natus
        repudiandae eius at excepturi alias saepe asperiores velit animi porro.
      </p>

      <div class="row q-gutter-sm">
        <q-btn color="secondary" no-caps style="border-radius: 25px"
          >Order Now</q-btn
        >
        <q-btn
          icon="play_arrow"
          no-caps
          flat
          style="border-radius: 25px; color: black"
          >Watch Video</q-btn
        >
      </div>
    </div>
    <q-img
      class="col"
      fit="contain"
      src="~assets/main/hero.svg"
      style="max-width: 500px"
    />
  </section>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HeadeSection",
});
</script>
