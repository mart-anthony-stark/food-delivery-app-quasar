<template>
  <q-page class="column q-pa-xl" style="color: #383c3e">
    <p class="text-h4">Popular Items</p>
    <p class="text-subtitle1">More Ordered Items</p>
    <div class="flex justify-center q-gutter-xl">
      <q-card
        class="item-card my-card column items-start q-pb-md"
        flat
        v-for="item in items"
        :key="item.id"
      >
        <img :src="item.img" />
        <q-card-section class="column q-gutter-sm">
          <div class="text-h6">{{ item.name }}</div>
          <div>{{ item.desc }}</div>
          <p class="q-pt-none text-h5">৳{{ item.price }}</p>
        </q-card-section>

        <q-btn icon="add" color="accent" class="q-ml-md add-btn" outline
          >Add</q-btn
        >
      </q-card>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PopularItems",
  data() {
    return {
      items: [
        {
          _id: 1,
          name: "Capuccino",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/capuccino.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 1050,
        },
        {
          _id: 2,
          name: "Bacon and egg sandwhich",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/bacon_egg.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 4599,
        },
        {
          _id: 3,
          name: "Capuccino",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/capuccino.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 1050,
        },
        {
          _id: 4,
          name: "Bacon and egg sandwhich",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/bacon_egg.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 4599,
        },
      ],
    };
  },
});
</script>

<style scoped>
.item-card {
  width: 270px;
  height: 450px;
}
.add-btn {
  position: absolute;
  bottom: 20px;
}
</style>
