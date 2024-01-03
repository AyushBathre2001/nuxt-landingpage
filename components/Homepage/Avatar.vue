<script setup>
const images = ref([
  "/images/avatar/ava1.png",
  "/images/avatar/ava1.png",
  "/images/avatar/ava1.png",
  "/images/avatar/ava1.png",
  "/images/avatar/ava1.png",
  "/images/avatar/ava1.png",
]);
</script>

<template>
  <div class="w-full py-16 flex items-center justify-center">
    <div class="max-w-screen-xl px-4 mx-auto flex lg:flex-row flex-col w-full h-full items-center justify-center ">
      <div class=" lg:w-[50%] w-full h-full lg:text-left text-center  flex flex-col items-center justify-center gap-3">
        <h1 class="md:text-5xl text-4xl font-bold leading-tight">
          <span class="text-blue-500">For Pros</span>, and the ones who want
          to become experts.
        </h1>
        <p class="text-sm font-medium text-[#83939C]">
          Whether you're a solo designer or part of a team, a junior or a
          senior, at an agency or a large organization, Prime has you covered.
        </p>
        <p class="text-sm font-medium text-[#83939C]">
          It's not about the number of components. With
          <span class="text-black"
            >top figma tricks & techniques, battle-tested design system
            approach</span
          >,
          Prime supercharges your skills and empowers you to work at warp
          speed.
        </p>
      </div>
      <div
        class="lg:w-[50%] w-full md:min-h-96 p-5 gap-5  flex flex-wrap items-center justify-center "
        
      >
        <img src="/images/avatar/ava1.png" class=" md:h-40 h-16 w-auto "/>
        <img src="/images/avatar/ava2.png" class=" md:h-40 h-16 w-auto "/>
        <img src="/images/avatar/ava3.png" class=" md:h-40 h-16 w-auto "/>
        <img src="/images/avatar/ava4.png" class=" md:h-40 h-16 w-auto "/>
        <img src="/images/avatar/ava5.png" class=" md:h-40 h-16 w-auto "/>
        <img src="/images/avatar/ava6.png" class=" md:h-40 h-16 w-auto "/>
    </div>
    </div>
  </div>
</template>

