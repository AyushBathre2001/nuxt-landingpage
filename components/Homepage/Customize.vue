<script setup>
const props = defineProps(["title1", "title2", "desc", "img"]);
</script>

<template>
  <div class="w-full py-20">
    <div class="max-w-screen-xl mx-auto px-4 flex flex-col gap-10">
      <div class="flex flex-col gap-1 lg:text-left text-center">
        <h1 class="md:text-5xl text-4xl text-[#000000] font-bold">
          {{ props.title1 }}
        </h1>
        <h1 class="md:text-5xl text-4xl text-[#4E616B] font-bold leading-tight">
          {{ props.title2 }}
        </h1>
        <p class="text-sm text-[#83939C]">{{ props.desc }}</p>
      </div>
      <img
        v-motion
        :initial="{ opacity: 0, y: 50 }"
        :delay="200"
        :visibleOnce="{
          opacity: 1,
          y: 0,
          transition: {
            duration: 1,
            type: 'spring',
            stiffness: 250,
            damping: 25,
            mass: 1.5,
          },
        }"
        :src="props.img"
        class="w-full h-auto"
        loading="lazy"
      />
    </div>
  </div>
</template>
