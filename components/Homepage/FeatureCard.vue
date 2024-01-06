<script setup>
const props = defineProps(["image", "label", "desc"]);
</script>

<template>
  <div
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
    class="w-full flex flex-col justify-center gap-5"
  >
    <div class="w-full">
      <img loading="lazy" class="w-full h-auto object-contain" alt="img" :src="props.image" />
    </div>
    <div class="text-sm font-bold">
      <p>{{ props.label }}</p>
      <p class="text-[#83939C]">{{ props.desc }}</p>
    </div>
  </div>
</template>
