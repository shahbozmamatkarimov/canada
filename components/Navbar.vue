<template>
    <nav class="flex items-center h-[70px]">
        <ul class="flex justify-between items-center w-full md:px-20 sm:px-10 px-5 py-5">
            <li data-aos="fade-down" class="text-xl leading-6 font-bold">
                Logo
            </li>
            <ul class="flex gap-6 font-semibold leading-6">
                <li data-aos="fade-down">
                    <router-link to="/login">Sign in</router-link>
                </li>
                <li data-aos="fade-left">
                    <router-link to="/login">Sign up</router-link></li>
            </ul>
        </ul>
    </nav>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>