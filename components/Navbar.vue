<template>
  <nav class="flex items-center h-[70px]">
    <ul
      class="flex justify-between items-center w-full md:px-20 sm:px-10 px-5 py-5"
    >
      <li data-aos="fade-down" class="text-xl leading-6 font-bold">
        <img src="@/public/nefa.svg" alt="">
      </li>
      <div class="flex space-x-3">
        <router-link to="/login">
          <Button
            class="px-8 xl:px-10 mt-2 whitespace-nowrap py-2 bg-inherit text-gradient border border-[#0c66ee]"
          >
            Sign in
          </Button>
        </router-link>
        <router-link to="/register">
          <Button
            class="px-8 xl:px-10 mt-2 whitespace-nowrap py-2 bg-gradient-to-r from-[#468ef9] to-[#0c66ee] text-white"
          >
            Sign Up
          </Button>
        </router-link>
      </div>
    </ul>
  </nav>
</template>

<script setup></script>

<style lang="scss" scoped></style>
