<template>
    <div class="w-full md:h-48 flex flex-col bg-[#171C1F] p-4 items-start gap-2 rounded-xl">
        <img :src="props.img" alt="" class="h-6 w-auto">
        <p class="text-[#FFFFFF] font-medium">{{ props.label }}</p>
        <p class="text-[#83939C] text-sm">{{ props.desc }}</p>
    </div>
</template>

<script setup>
    const props = defineProps(["img","label","desc"])
</script>

