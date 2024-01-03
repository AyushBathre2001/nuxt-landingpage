<script setup>
const props = defineProps(["image","label","desc"])
</script>

<template>
    <div class="w-full flex flex-col justify-center gap-5 ">
        <div class="w-full">
            <img class="w-full h-auto object-contain" alt="img" :src="props.image"/>
        </div>
        <div class="text-sm font-bold">
            <p>{{ props.label }}</p>
            <p class="text-[#83939C]">{{ props.desc }}</p>
        </div>

    </div>
</template>


