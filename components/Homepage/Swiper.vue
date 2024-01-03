<script setup>
import { ref } from 'vue';
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

const images = ref([
  '/images/company/co1.svg',
  '/images/company/co2.svg',
  '/images/company/co3.svg',
  '/images/company/co4.svg',
  '/images/company/co5.svg',
  '/images/company/co6.svg',
  '/images/company/co7.svg',
  '/images/company/co8.svg',
]);

const onSwiper = (swiper) => {
  console.log(swiper);
};

const onSlideChange = () => {
  console.log('slide change');
};
</script>

<template>
    <div class="max-w-screen-xl mx-auto h-[35vh]  items-center md:flex hidden justify-center cursor-grab">
  <swiper
    :slides-per-view="7"
    :space-between="50"
    :loop="true"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide v-for="(img, index) in images" :key="index">
      <div class="h-10">
        <img :src="img" alt="Company Logo" class="h-full w-auto" />
      </div>
    </swiper-slide>
  </swiper>
</div>
</template>