<script setup>
  const data = ref([
    {
      label:"How to import Prime into Figma",
      desc:" Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
    },
    {
      label:"Do I need to have paid Figma plan to work with Prime?",
      desc:" Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
    },
    {
      label:"Do I need to be Figma pro?",
      desc:" Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
    },
    {
      label:"How do i get an update of the kit?",
      desc:" Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
    },
    {
      label:"Do you offer Purchase Power Parity discounts?",
      desc:" Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
    },
    {
      label:"Do you offer discounts for Students & Teachers?",
      desc:" Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat."
    },
  ])
</script>


<template>
  <div class="w-full py-16">
    <div class="max-w-screen-xl mx-auto px-4 flex flex-col gap-10">
      <div class="text-center lg:text-left">
        <h1 class="md:text-5xl text-4xl font-bold">Have a question?</h1>
        <h1 class="md:text-5xl text-4xl font-bold text-[#4E616B]">FAQ</h1>
      </div>
      <div class="m-2 space-y-2">
        <div v-for="(item,index) in data" :key="index">
          <div
          class="group flex flex-col gap-2 rounded-lg bg-[#F4F5F6] p-5 text-[#000000]"
          tabindex="1"
        >
          <div class="flex cursor-pointer items-center justify-between">
            <span class="text-sm font-semibold">
              {{ item.label }}</span
            >
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/9/96/Chevron-icon-drop-down-menu-WHITE.png"
              class="h-2 w-3 transition-all duration-500 group-focus:-rotate-180"
            />
          </div>
          <div
            class="invisible h-auto max-h-0 items-center opacity-0 transition-all group-focus:visible group-focus:max-h-screen group-focus:opacity-100 group-focus:duration-1000"
          >
          {{ item.desc }}
          </div>
        </div>
        </div>
       
      </div>
    </div>
  </div>
</template>
