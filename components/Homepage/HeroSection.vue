<script setup>
  import { ref, onMounted } from 'vue';

  const isMounted = ref(false);

  onMounted(() => {
    isMounted.value = true;
  });
</script>

<template>
  <div class="w-full h-screen bg-[url('/images/hero.jpg')] bg-cover">
    <div
      v-if="isMounted"
      class="max-w-screen-xl mx-auto px-4 flex flex-col gap-5 items-center justify-center text-center h-full"
    >
      <div class="flex flex-col gap-3">
        <img src="/images/logo.png" alt="logo" class="h-16 w-16" />
        <p
          v-motion
          :initial="{ opacity: 0, y: 50 }"
          :enter="{ opacity: 1, y: 0,
          transition:{
            duration:500
          } }"
          :delay="500"
          class="text-lg font-bold"
        >
          Prime 5
        </p>
      </div>
      <div class="flex flex-col gap-3">
        <h1
          v-motion
          :initial="{ opacity: 0, y: 50 }"
          :enter="{ opacity: 1, y: 0,transition:{
            duration:500
          } }"
          :delay="700"
          class="md:text-5xl text-4xl font-bold leading-tight"
        >
          Figma Design System <br />
          at it's finest
        </h1>
        <p
          v-motion
          :initial="{ opacity: 0, y: 50 }"
          :enter="{ opacity: 1, y: 0,transition:{
            duration:500
          } }"
          :delay="800"
          class="font-medium text-[#4E616B]"
        >
          Supercharge your design workflow with top Figma & Design System
          techniques. <br />
          Powerful components with tokens to complete every project 10x faster.
          <br />
          It's far more than just a UI Kit.
        </p>
      </div>
      <div class="flex gap-3">
        <button class="px-5 py-3 rounded-xl bg-blue-500 text-white">
          Get it now
        </button>
        <button class="px-5 py-3 rounded-xl bg-[#F4F5F6] text-black">
          Live preview
        </button>
      </div>
    </div>
  </div>
</template>

<style scoped>
  [v-motion]:not(.motion-enter-active) {
    opacity: 0;
    transform: translateY(50px);
  }
</style>
