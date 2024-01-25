<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
import About from './components/About.vue'
import Features from './components/Features.vue'
</script>

<template>
  <div class="head">
    <header class="flex justify-center space-x-10 p-2 backdrop-blur-sm text-white">
      <div class="justify-center mr-20"><img alt="Vue logo" class="logo" src="/logo.webp" width="110" height="90" /></div>

      <div class="my-auto">

        <nav class="text-xl justify-center space-x-10">
          <RouterLink to="/" class="p-2">About</RouterLink>
          <RouterLink to="/about" class="p-2">Communities</RouterLink>
          <RouterLink to="/about" class="p-2">The company</RouterLink>
          <RouterLink to="/about" class="p-2">Contact us</RouterLink>
          <a href="#" class="p-5 bg-orange-400 font-medium rounded-full">Get The App</a>
        </nav>
      </div>
    </header>

    <RouterView />
    <div class="flex-col justify-center text-5xl space-y-5 p-5 mt-48 mb-48 text-center text-white font-bold">
      <p>Your Guide To</p>
      <p>Shipping Industry</p>
    </div>
    <About />
    <Features />
  </div>
</template>

<style scoped>
.head {
  height: 100vh;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.2)), url('/cargo.jpg') no-repeat center fixed;
}
</style>
