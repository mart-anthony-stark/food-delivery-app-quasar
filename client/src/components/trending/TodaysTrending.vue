<template>
  <q-page class="q-pa-xl flex= justify-center" style="color: #383c3e">
    <div class="container flex justify-center column">
      <p class="text-h4">Todays Trending</p>
      <p class="text-subtitle1">People loves it most the past week...</p>
      <div class="row q-gutter-md">
        <div class="col">
          <q-carousel
            swipeable
            animated
            v-model="slide"
            thumbnails
            infinite
            autoplay
            arrows
          >
            <q-carousel-slide :name="1" img-src="~assets/basomoti.svg" />
            <q-carousel-slide :name="2" img-src="~assets/basomoti.svg" />
            <q-carousel-slide :name="3" img-src="~assets/basomoti.svg" />
            <q-carousel-slide :name="4" img-src="~assets/basomoti.svg" />
          </q-carousel>
        </div>
        <div class="col-5 column justify-between">
          <div>
            <p class="text-h6">Basomoti Kacchi Biriyani</p>
            <p class="text-h5">৳1,050</p>
            <div class="row flex items-center q-gutter-lg">
              <q-rating
                v-model="ratingModel"
                size="2em"
                :max="5"
                color="primary"
              />
              <div class="q-diva-none">5.0 out of (1256) Reviews</div>
            </div>
          </div>

          <div>
            <div class="text-h5 q-ma-none">Select Quantity</div>
            <div class="flex q-gutter-md q-pt-md">
              <q-btn outline label="1" />
              <q-btn outline label="2" />
              <q-btn outline label="3" />
              <q-btn outline label="4" />
            </div>
            <q-btn-group class="q-pt-md" outline>
              <q-btn class="q-px-xl q-py-md" outline>
                <q-icon name="favorite_outlined" color="red" />
              </q-btn>
              <q-btn class="q-px-xl q-py-md" outline>
                <q-icon name="shopping_cart" color="primary" />
              </q-btn>
            </q-btn-group>
          </div>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      slide: ref(1),
      ratingModel: ref(4),
    };
  },
};
</script>
