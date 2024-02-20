<template>
  <Mainlayouts class="">
    <div class="flex flex-col gap-y-12">
      <hero-section />
      <HomeBenefits />
      <indexVue />
    </div>
    <Featured />
    <customer />
    <Refer />
    <Join />
    <Partners />
  </Mainlayouts>
</template>

<script setup>
import HeroSection from "~/components/Home/HeroSection.vue";
import Mainlayouts from "../layouts/Mainlayouts.vue";
import indexVue from "~/components/Home/Products/index.vue";
import Featured from "~/components/Home/Featured.vue";
import Customer from "~/components/Home/Customer.vue";
import Refer from "~/components/Home/Refer.vue";
// import JoinVue
import Join from "~/components/Home/Join.vue";
// import PartnersVue
import Partners from "~/components/Home/Partners.vue";
</script>

<style lang="scss" scoped>
</style>