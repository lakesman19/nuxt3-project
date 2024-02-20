<template>
  <div
    class="w-full bg-[white] flex justify-center relative items-center py-12"
  >
    <div class="w-[85%] flex flex-col gap-6">
      <div
        class="flex flex-col justify-center items-center gap-y-3 text-center w-full"
      >
        <h1 class="text-[#0A2240] text-4xl font-bold md:w-[60%]">
          Our users are in love with us
        </h1>
        <p class="text-lg text-[#1A1A38] font[40] md:w-[60%]">
          Since we launched we have helped people from all walks of life grow
          and achieve their personal financial goals.
        </p>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div
          v-for="(item, index) in customer"
          :key="index"
          :style="{ backgroundColor: item.bg }"
          class="p-6 rounded-lg shadow-md"
        >
          <p class="text-base text-[#1A1A38]">{{ item.p }}</p>
          <p class="text-[#0A2240] text-lg font-semibold mt-4">
            {{ item.name }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { customer } from "~/assets/Dummy";
</script>

<style lang="scss" scoped>
</style>