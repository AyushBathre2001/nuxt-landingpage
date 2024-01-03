<script setup>
const data = ref([
  {
    img: "/images/practice/img1.svg",
    label: "Semantic tokens",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img2.svg",
    label: "Proper component exposure",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img3.svg",
    label: "Component excellence",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img4.svg",
    label: "4pt soft-grid system",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img5.svg",
    label: "True accessibility in mind",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img6.svg",
    label: "Universal typography",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img7.svg",
    label: "Variables & styles",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img8.svg",
    label: "Top-notch effects",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img9.svg",
    label: "Auto layout",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img10.svg",
    label: "Variants & properties",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img11.svg",
    label: "Phosphor Icons",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
  {
    img: "/images/practice/img12.svg",
    label: "Dark & light modes",
    desc: "Meaningful styling is the foundation of design systems. Use techniques from world-class design systems, not random UI kits.",
  },
]);
</script>

<template>
  <div class="w-full bg-black">
    <div class="max-w-screen-xl mx-auto px-4 flex flex-col">
      <div class="flex flex-col items-center md:text-left text-center justify-center py-20">
        <h1 class="md:text-5xl text-4xl text-[#FFFFFF] font-bold">Best practices</h1>
        <h1 class="md:text-5xl text-4xl text-[#A0ADB4] font-bold">
          World-class standards inside
        </h1>
      </div>
      <div class="w-full grid md:grid-cols-3 grid-cols-1 gap-5 py-10">
        <div v-for="(item, index) in data" :key="index">
          <HomepagePracticeCard
            :img="item.img"
            :label="item.label"
            :desc="item.desc"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
