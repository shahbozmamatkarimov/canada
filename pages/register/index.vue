<template>
  <main class="flex items-center justify-center bg-[#9747FF] min-h-screen">
    <section
      class="bg-[#FFA629] sm:h-auto h-[100vh] sm:rounded-[10px] w-[640px]"
    >
      <ul class="flex justify-between items-center h-10">
        <li
          @click="store.registerType = 'Customer'"
          :class="
            store.registerType != 'Business' ? 'bg-[#F24822] text-white' : ''
          "
          class="flex items-center cursor-pointer duration-500 justify-center h-full w-full rounded-[10px]"
        >
          Customer register
        </li>
        <li
          @click="store.registerType = 'Business'"
          :class="
            store.registerType == 'Business' ? 'bg-[#F24822] text-white' : ''
          "
          class="flex items-center cursor-pointer duration-500 justify-center h-full w-full rounded-[10px]"
        >
          Business register
        </li>
      </ul>
      <form class="md:p-16 sm:p-10 p-5 py-16">
        <!-- <h1 class="text-2xl font-bold">Your logo</h1> -->
        <!-- <h1 class="text-4xl font-bold mt-[13px] mb-[26px]">register</h1> -->

        <div class="space-y-[30px]">
          <div class="space-y-[5px]">
            <label for="email">Email</label><br />
            <input
              class="h-[50px] px-5 rounded-[10px] w-full"
              autocomplete="email"
              type="email"
              id="email"
              placeholder="username@gmail.com"
            />
          </div>
          <div class="space-y-[5px]">
            <label for="password">Password</label><br />
            <div class="relative">
              <input
                class="h-[50px] px-5 pr-16 rounded-[10px] w-full"
                autocomplete="new-password"
                :type="store.passType ? 'text' : 'password'"
                id="password"
                placeholder="Password"
              />
              <img
                v-if="!store.passType"
                @click="store.passType = true"
                class="absolute cursor-pointer top-3.5 right-5"
                src="@/assets/icons/hidden.svg"
                alt="Google"
              />
              <img
                v-if="store.passType"
                @click="store.passType = false"
                class="absolute cursor-pointer top-3.5 right-5"
                src="@/assets/icons/show.svg"
                alt="Google"
              />
            </div>
          </div>
        </div>
        <button
          class="flex mt-[30px] items-center justify-center h-[50px] bg-[#F24822] rounded-[10px] w-full text-white text-xl font-bold"
          type="submit"
        >
          Sign up
        </button>
        <p class="text-sm text-center my-8">or continue with</p>
        <div class="flex gap-[25px]">
          <div
            class="flex items-center justify-center cursor-pointer w-full h-[50px] bg-white rounded-[10px]"
          >
            <img src="@/assets/auth/google.svg" alt="Google" />
          </div>
          <div
            class="flex items-center justify-center cursor-pointer w-full h-[50px] bg-white rounded-[10px]"
          >
            <img src="@/assets/auth/github.svg" alt="Github" />
          </div>
          <div
            class="flex items-center justify-center cursor-pointer w-full h-[50px] bg-white rounded-[10px]"
          >
            <img src="@/assets/auth/facebook.svg" alt="Facebook" />
          </div>
        </div>
        <p class="mt-8 text-center text-sm text-gray-800">
            Did you have already account?
          <router-link class="font-semibold text-black" to="/register"
            >Login here</router-link
          >
        </p>
      </form>
    </section>
  </main>
</template>

<script setup>
definePageMeta({
  registerType: "Business",
  layout: false,
});

const store = reactive({
  passType: false,
});
</script>

<style lang="scss" scoped></style>
