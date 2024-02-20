<template>
  <div class="flex justify-center items-center flex-col w-full gap-y-8">
    <div class="w-[85%]">
      <div
        class="flex justify-center items-center md:justify-start md:items-start gap-y-1 flex-col"
      >
        <h1
          class="text-[#0A2240] text-center md:text-start text-3xl md:text-5xl font-[700] md:w-[65%]"
        >
          Meet Vale Products Tailored For You
        </h1>
        <div class="h-[5px] w-[150px] bg-[#0267FD] rounded-lg"></div>
      </div>
    </div>
    <div class="w-full">
      <targets />
      <vaults />
    </div>
  </div>
</template>

<script setup>
import Targets from "./Targets.vue";
import Vaults from "./Vaults.vue";
</script>

<style lang="scss" scoped>
</style>