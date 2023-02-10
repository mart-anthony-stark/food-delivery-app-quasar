<template>
  <q-page class="column q-pa-xl" style="color: #383c3e">
    <p class="text-h4">Popular Items</p>
    <p class="text-subtitle1">More Ordered Items</p>
    <div class="flex justify-center q-gutter-xl">
      <ItemCard v-for="item in items" :key="item._id" :item="item" />
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import ItemCard from "./ItemCard.vue";

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
        {
          _id: 5,
          name: "Capuccino",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/capuccino.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 1050,
        },
        {
          _id: 6,
          name: "Bacon and egg sandwhich",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/bacon_egg.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 4599,
        },
        {
          _id: 7,
          name: "Capuccino",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/capuccino.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 1050,
        },
        {
          _id: 8,
          name: "Bacon and egg sandwhich",
          img: "https://github.com/mart-anthony-stark/food-delivery-app-quasar/blob/master/client/src/assets/popular/bacon_egg.jpg?raw=true",
          desc: "Served with Lorem ipsum dolor sit.",
          price: 4599,
        },
      ],
    };
  },
  components: { ItemCard },
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
