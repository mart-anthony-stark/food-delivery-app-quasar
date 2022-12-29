<template>
  <q-card class="item-card my-card column items-start q-pb-md" flat>
    <q-img :src="item.img" />
    <q-card-section class="column q-gutter-sm">
      <div class="text-h6">{{ item.name }}</div>
      <div>{{ item.desc }}</div>
      <p class="q-pt-none text-h5">৳{{ item.price }}</p>
    </q-card-section>

    <q-btn icon="add" color="accent" class="q-ml-md add-btn" outline>Add</q-btn>
  </q-card>
</template>

<script setup>
const props = defineProps({
  item: {
    name: String,
    desc: String,
    img: String,
    price: Number,
  },
});
</script>
