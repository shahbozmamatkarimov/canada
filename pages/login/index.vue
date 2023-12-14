<template>
  <main
    class="flex font-bold items-center justify-center bg-[#6533a7] min-h-screen h-full"
  >
    <section class="register z-10 sm:h-auto h-[100vh] sm:rounded-3xl w-[640px]">
      <div class="flex justify-between items-center h-10">
        <Button
          @click="store.loginType = 'Customer'"
          :class="
            store.loginType != 'Business'
              ? 'bg-gradient-to-r from-[#468ef9] to-[#0c66ee] text-white'
              : 'text-gradient border border-[#0c66ee]'
          "
          class="flex items-center cursor-pointer duration-1000 justify-center h-full w-full rounded-full"
        >
          Customer login
        </Button>
        <Button
          @click="store.loginType = 'Business'"
          :class="
            store.loginType == 'Business'
              ? 'bg-gradient-to-r from-[#468ef9] to-[#0c66ee] text-white'
              : 'text-gradient border border-[#0c66ee]'
          "
          class="flex items-center cursor-pointer duration-1000 justify-center h-full w-full rounded-full"
        >
          Business login
        </Button>
      </div>
      <router-link
        to="/"
        data-aos="fade-down"
        class="block text-xl leading-6 py-5 font-bold"
      >
        <img class="mx-auto" src="@/public/nefa.svg" alt="" />
      </router-link>
      <form class="md:p-16 md:pt-0 pt-0 text-white sm:p-10 p-5 py-16">
        <div class="space-y-[30px]">
          <div class="space-y-[5px]">
            <label for="email">Email</label><br />
            <input
              class="h-[50px] px-5 rounded-[10px] w-full bg-transparent border border-[#0c66ee]"
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
                class="h-[50px] px-5 pr-16 rounded-[10px] w-full bg-transparent border border-[#0c66ee]"
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
        <router-link to="/login" class="block mt-2 mb-[30px]"
          >Forgot Password?</router-link
        >
        <button
          data-aos="fade-up"
          data-aos-delay="1000"
          class="flex items-center justify-center h-[50px] bg-gradient-to-r from-[#468ef9] to-[#0c66ee] rounded-full w-full text-white text-xl font-bold"
          type="submit"
        >
          Sign in
        </button>
        <p class="text-sm text-center my-8">or continue with</p>
        <div class="flex gap-[25px]">
          <div
            data-aos="fade-up"
            data-aos-delay="500"
            class="flex items-center justify-center cursor-pointer w-full h-[50px] bg-white rounded-[10px]"
          >
            <img src="@/assets/auth/google.svg" alt="Google" />
          </div>
          <div
            data-aos="fade-up"
            data-aos-delay="700"
            class="flex items-center justify-center cursor-pointer w-full h-[50px] bg-white rounded-[10px]"
          >
            <img src="@/assets/auth/github.svg" alt="Github" />
          </div>
          <div
            data-aos="fade-up"
            data-aos-delay="900"
            class="flex items-center justify-center cursor-pointer w-full h-[50px] bg-white rounded-[10px]"
          >
            <img src="@/assets/auth/facebook.svg" alt="Facebook" />
          </div>
        </div>
        <p class="mt-8 text-center text-sm text-white/60">
          Don’t have an account yet?
          <router-link
            class="font-semibold whitespace-nowrap text-white"
            to="/register"
            >Register here</router-link
          >
        </p>
      </form>
    </section>

    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/ellipse-2.png"
      class="block absolute top-4 sm:top-20 right-64 sm:right-96 xl:right-[25rem] w-6"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/ellipse-2.png"
      class="block absolute top-4 sm:top-96 right-20 sm:right-96 xl:right-[20rem] w-6"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/ellipse-3.png"
      class="block absolute bottom-56 right-24 w-6"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/ellipse-3.png"
      class="block absolute bottom-56 right-[32rem] w-6"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/ellipse-3.png"
      class="block absolute bottom-80 md:left-[40rem] left-[16rem] w-6"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/ellipse-3.png"
      class="block absolute bottom-56 left-24 w-6"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/ellipse-3.png"
      class="block absolute top-72 md:left-96 left-48 w-6"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/star.png"
      class="block absolute top-20 sm:top-28 right-16 lg:right-0 lg:left-[30rem] w-8"
    />
    <img
      data-aos="fade-up"
      data-aos-delay="300"
      src="@/assets/img/pattern/star.png"
      class="block absolute top-20 sm:top-28 right-16 lg:right-0 lg:left-[10rem] w-8"
    />
  </main>
</template>

<script setup>
definePageMeta({
  layout: false,
});

const store = reactive({
  loginType: "Business",
  passType: false,
});
</script>

<style lang="scss" scoped>
.register {
  border: 3px solid rgba(88, 130, 193, 0.28);
  background: rgba(88, 130, 193, 0.28);
  backdrop-filter: blur(12.5px);
}
</style>
