<template>
  <main class="flex items-center min-h-[calc(100vh_-_70px)]">
    <section class="relative max-w-screen-xl px-4 sm:px-8 mx-auto grid grid-cols-12 gap-x-6 overflow-hidden">
      <div
        class="col-span-12 lg:col-span-6 mt-12 xl:mt-10 space-y-4 sm:space-y-6 px-6 text-center sm:text-left"
      >
        <router-link to="/register"
          data-aos="fade-right"
          data-aos-once="true"
          class="text-base text-gradient font-semibold uppercase"
          >Sign Up Today</router-link
        >
        <h1
          data-aos="fade-right"
          data-aos-once="true"
          class="text-[2.5rem] sm:text-5xl xl:text-6xl font-bold leading-tight capitalize sm:pr-8 xl:pr-10"
        >
          The World's
          <span class="text-header-gradient">Fastest Growing</span> Crypto Web
          App
        </h1>
        <p
          data-aos="fade-down"
          data-aos-once="true"
          data-aos-delay="300"
          class="paragraph hidden sm:block"
        >
          Buy and sell 200+ cryptocurrencies with 20+ flat currencies using bank
          transfers or your credit/debit card.
        </p>
        <div
          data-aos="fade-up"
          data-aos-once="true"
          data-aos-delay="700"
          class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4 mt-2"
        >
          <Button
            class="max-w-full px-8 py-4 bg-gradient-to-r from-[#468ef9] to-[#0c66ee] border border-[#0c66ee] text-white"
          >
            Get Started
          </Button>
          <Button
            class="max-w-full px-6 py-4 text-gradient border border-[#0c66ee] flex items-center justify-center"
          >
            <span>Download App</span>
            <ChevronDownIcon :size="20" class="mt-1 text-[#0c66ee]" />
          </Button>
        </div>
      </div>
      <div class="hidden sm:block col-span-12 lg:col-span-6">
        <div class="w-full">
          <img
            data-aos="fade-up"
            data-aos-once="true"
            src="@/assets/img/hero-image.webp"
            class="-mt-4"
            alt=""
          />
        </div>
      </div>
      <img
        data-aos="fade-up"
        data-aos-delay="300"
        src="@/assets/img/pattern/ellipse-1.png"
        class="hidden sm:block absolute bottom-12 xl:bottom-16 left-4 xl:left-0 w-6"
      />
      <img
        data-aos="fade-up"
        data-aos-delay="300"
        src="@/assets/img/pattern/ellipse-2.png"
        class="hidden sm:block absolute top-4 sm:top-10 right-64 sm:right-96 xl:right-[32rem] w-6"
      />
      <img
        data-aos="fade-up"
        data-aos-delay="300"
        src="@/assets/img/pattern/ellipse-3.png"
        class="hidden sm:block absolute bottom-56 right-24 w-6"
      />
      <img
        data-aos="fade-up"
        data-aos-delay="300"
        src="@/assets/img/pattern/star.png"
        class="hidden sm:block absolute top-20 sm:top-28 right-16 lg:right-0 lg:left-[30rem] w-8"
      />
    </section>
    <!-- <section
      class="sm:flex justify-between items-center lg:gap-40 gap-10 lg:py-10 py-5 w-full"
    >
      <div
        data-aos="fade-right"
        class="lg:space-y-[30px] space-y-[15px] sm:w-full w-[70%]"
      >
        <h1
          data-aos="fade-right"
          class="sm:text-[calc(100vw/40)] text-xl sm:leading-[calc(100vw/35)] leading-6 font-bold"
        >
          Welcome to my new Creative Website!
        </h1>
        <p class="sm:text-[calc(100vw/70)] leading-7 text-sm text-[#1D1D1D]">
          Kirit Goti is a designer focused on building brands and creating
          digital experiences — currently working at Hoca
        </p>
        <button
          class="bg-[#1D1D1D] text-white md:px-5 px-3 md:py-3 py-2 rounded-[10px] font-semibold sm:text-[calc(100vw/80)] text-xs"
        >
          Let’s Get Started
        </button>
      </div>
      <div data-aos="fade-down" class="flex sm:justify-end min-w-[50%]">
        <img
          class="sm:h-[calc(100vh_-_200px)] sm:mt-0 mt-8 lg:min-h-[380px] min-h-[200px]"
          src="@/assets/images/get_started.svg"
          alt=""
        />
      </div>
    </section> -->
  </main>
</template>

<script setup></script>

<style lang="scss">
.text-header-gradient {
  background: rgb(57, 132, 244);
  background: linear-gradient(
    169.4deg,
    #3984f4 -6.01%,
    #0cd3ff 36.87%,
    #2f7cf0 78.04%,
    #0e65e8 103.77%
  );
  background-clip: text;
  -webkit-text-fill-color: transparent;
}

.text-gradient {
  background: linear-gradient(136.91deg, #468ef9 -12.5%, #0c66ee 107.5%);
}
.text-gradient {
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>
