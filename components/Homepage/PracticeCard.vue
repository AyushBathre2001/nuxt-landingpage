<template>
    <div  v-motion
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
    }" class="w-full md:h-48 flex flex-col bg-[#171C1F] p-4 items-start gap-2 rounded-xl">
        <img loading="lazy" :src="props.img" alt="" class="h-6 w-auto">
        <p class="text-[#FFFFFF] font-medium">{{ props.label }}</p>
        <p class="text-[#83939C] text-sm">{{ props.desc }}</p>
    </div>
</template>

<script setup>
    const props = defineProps(["img","label","desc"])
</script>

