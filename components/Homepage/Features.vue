<script setup>
const data = ref([
  {
    layout: 1,
    value: [
      {
        img: "/images/features/bg.jpg",
        label: "Robust UI library",
        desc: "3,100+ of easy to customize, pixel-perfect components crafted with the best practices, and tokens.",
      },
    ],
  },
  {
    layout: 2,
    value: [
      {
        img: "/images/features/f1.jpg",
        label: "Smart tokens & styles",
        desc: "Prime is tailored to use real design system tokens structure, with Figma variables",
      },
      {
        img: "/images/features/f2.jpg",
        label: "Easy customization",
        desc: "You customize only key colors, and see results propagated through entire design system.",
      },
    ],
  },

  {
    layout: 1,
    value: [
      {
        img: "/images/features/f3.jpg",
        label: "The best Figma practices",
        desc: "Knowledge, tips & tricks gained when mastering of every new Figma feature - all included in the kit.",
      },
    ],
  },
  {
    layout: 2,
    value: [
      {
        img: "/images/features/f4.jpg",
        label: "Supafast workflow",
        desc: "Prime offers components that you exactly need, nothing more, for fast and effcient use.",
      },
      {
        img: "/images/features/f5.jpg",
        label: "Best of design systems",
        desc: "Years working with real design systems means handy patterns, not considered in other kits",
      },
    ],
  },
]);
</script>

<template>
    <div class="max-w-screen-xl px-4 py-20 mx-auto flex flex-col items-center justify-center">
      <div class="text-center">
        <h1 class="md:text-5xl text-4xl font-bold">No-fluff.</h1>
        <h1 class="md:text-4xl text-3xl font-bold text-[#4E616B]">Here is what you get</h1>
      </div>
      <div v-for="(item, index) in data" :key="index" class="flex flex-col gap-20 mt-16">
        <div v-if="item.layout === 1" v-for="(val, ind) in item.value" :key="ind">
          <HomepageFeatureCard :image="val.img" :desc="val.desc" :label="val.label" />
        </div>
        <div v-if="item.layout === 2" class="w-full grid md:grid-cols-2 grid-cols-1 gap-4">
          <HomepageFeatureCard
            v-for="(val2, ind2) in item.value"
            :key="ind2"
            :image="val2.img"
            :desc="val2.desc"
            :label="val2.label"
            class="w-full" 
          />
        </div>
      </div>
    </div>
  </template>

