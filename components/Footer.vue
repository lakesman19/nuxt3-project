<template>
  <div
    class="w-[100%] flex flex-col justify-center items-center bg-[#0267FD] font1 py-9 mt-9"
  >
    <div class="w-[85%] text-white flex justify-center flex-col gap-y-4">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-y-3">
        <div class="w-[100%]">
          <div class="w-1/2">
            <img
              src="/assets/images/Logo.png"
              alt="website logo"
              class="object-fit w-[50%] h-full"
            />
          </div>
          <span>Savings, Payments, Loans</span>
        </div>

        <div class="flex flex-col gap-y-3 md:gap-y-6">
          <h2 class="font-bold">Quick</h2>
          <ul class="gap-2 flex flex-col">
            <li>
              <NuxtLink to="">Our Story</NuxtLink>
            </li>
            <li>
              <NuxtLink to="">FAQs</NuxtLink>
            </li>
            <li>
              <NuxtLink to="">Media</NuxtLink>
            </li>
          </ul>
        </div>
        <div class="flex flex-col gap-y-3 md:gap-y-6">
          <h2 class="font-bold">Legals</h2>
          <ul class="gap-2 flex flex-col">
            <li>
              <NuxtLink to="">Terms & Conditions</NuxtLink>
            </li>
            <li>
              <NuxtLink to="">Privacy Policy</NuxtLink>
            </li>
          </ul>
        </div>
        <div class="flex flex-col gap-y-3 md:gap-y-6">
          <h2 class="font-bold">Contact Us</h2>
          <div class="gap-2 flex flex-col w-full">
            <div class="flex gap-4 items-center w-full">
              <span class="text-lg">
                <img src="/assets/images/Vector2.png" alt="" />
              </span>
              <span class="break-all">
                UAC Building, 1-5 Odunlami St, Lagos Island, Lagos
              </span>
            </div>
            <div class="flex gap-4 items-center w-full">
              <span class="text-lg">
                <img src="/assets/images/Vector.png" alt="" />
              </span>
              <span>+234 812 345 6789</span>
            </div>
            <div class="flex gap-4 items-center w-full">
              <span class="text-lg">
                <img src="/assets/images/mail 1.png" alt="" />
              </span>
              <span>hello@vale.ng</span>
            </div>
            <div class="flex gap-2 items-center w-full">
              <span class="">
                <img src="/assets/images/Vector3.png" alt="" />
              </span>
              <span class="">
                <img src="/assets/images/Vector4.png" alt="" />
              </span>
              <span class="">
                <img src="/assets/images/bxl-twitter.svg.png" alt="" />
              </span>
              <!-- <span class="">
                <img src="/assets/images/bxl-whatsapp-square.svg.png" alt="" />
              </span> -->
            </div>
          </div>
        </div>
      </div>
      <div
        class="hidden md:block border-top border-white w-full border-[1px]"
      ></div>
      <p class="hidden md:block">
        Vale is a Mobile Bank provider, regulated by the Central Bank of
        Nigeria(CBN). Dollar investments are offered under a reseller
        partnership with Anchoria Asset Management Limited – a SEC-licensed
        asset management company. Deposit accounts are issued and managed by
        CBN-licensed deposit money banks
      </p>
      <span class="text-center md:text-left">
        2019 © All rights reserved by Vale Finance
      </span>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
</style>