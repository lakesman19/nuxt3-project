<template>
  <div
    class="w-[100%] flex justify-center items-center bg-[#0267FD] py-3 transition-all duration-75 fixe z-[999]"
  >
    <div class="flex justify-between items-center w-[85%]">
      <NuxtLink to="/">
        <img src="/assets/images/valeLogowhite.svg" alt="" srcset="" />
      </NuxtLink>
      <ul
        class="md:flex items-center justify-center gap-5 text-white hidden capitalize"
      >
        <li><NuxtLink to=""> personal </NuxtLink></li>
        <li><NuxtLink to=""> Business </NuxtLink></li>
        <li><NuxtLink to=""> Company </NuxtLink></li>
        <li><NuxtLink to=""> Help </NuxtLink></li>
      </ul>
      <div class="md:flex items-center gap-3 font1 text-white hidden">
        <NuxtLink class=""> Sign In </NuxtLink>
        <NuxtLink
          class="bg-white p-2 text-[#0267FD] rounded-md font-medium border-none outline-none"
          >Create Account</NuxtLink
        >
      </div>
      <div class="flex md:hidden" @click="toggleMenu">
        <Icon name="mdi:hamburger-menu" color="white" size="25" />
      </div>
    </div>
    <div
      v-if="isMenuOpen"
      class="mediumscreen flex justify-center gap-3 items-center md:hidden"
    >
      <span
        class="top-0 right-0 absolute text-2xl p-8 border-black"
        @click="closeMenu"
      >
        <Icon name="mingcute:close-line" color="#0267FD" size="25" />
      </span>
      <ul
        class="flex items-center flex-col justify-center gap-3 font1 text-black font-medium w-full"
      >
        <li><NuxtLink to=""> personal </NuxtLink></li>
        <li><NuxtLink to=""> Business </NuxtLink></li>
        <li><NuxtLink to=""> Company </NuxtLink></li>
        <li><NuxtLink to=""> Help </NuxtLink></li>
      </ul>
      <div class="md:flex items-center gap-3 font1 text-white hidden">
        <NuxtLink class="sign"> Sign In </NuxtLink>
        <NuxtLink
          class="bg-white p-2 text-[#0267FD] login rounded-md font-medium border-none outline-none"
          >Create Account</NuxtLink
        >
      </div>
    </div>
  </div>
</template>

<script setup>
const isMenuOpen = ref(false);
const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
  console.log("yes", isMenuOpen.value);
};
const closeMenu = () => {
  isMenuOpen.value = false;
};
</script>

<style scoped>
.mediumscreen {
  /* display: flex; */
  border-radius: 3px;
  box-shadow: 0 1px 50px 0 rgba(33, 51, 67, 0.12);
  background-color: white;
  right: -100%;
  text-align: center;
  top: 0;
  transition: right 0.8s ease-in-out;
  width: 100%;
  padding: 2rem;
  z-index: 1000;
  min-height: 400px;
  color: black;
  text-transform: capitalize;

  position: fixed;
  animation: showmenu 300ms ease forwards;
}
@keyframes showmenu {
  from {
    right: -100%; /* Start from the right, off the screen */
  }
  to {
    right: 0; /* Slide in from the right */
  }
}
.login {
  border: 1px solid #0267fd !important;
  color: #0267fd !important;
  border-radius: 8px;
  font-weight: 600;
  text-transform: capitalize;
}

.sign {
  background-color: #0267fd !important;
  border: 1px solid #0267fd !important;
  color: #fcfcfc !important;
  border-radius: 8px;
  font-weight: 600;
  text-transform: capitalize;
}
</style>
