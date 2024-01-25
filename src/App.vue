<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
import About from './components/About.vue'
import Features from './components/Features.vue'
import Liner from './components/Liner.vue'
import Products from './components/Products.vue'
import Information from './components/Information.vue'
import Footer from './components/Footer.vue'
function m() {
  const menu = document.querySelector("#menu")
  menu.classList.toggle("active")
}
</script>

<template>
  <div class="head">
    <!--mob-->
    <nav class="nav bg-gray-500 bg-transparent text-gray-200 md:hidden sticky top-0 z-10 justify-between font-semibold ">
      <div class="flex justify-between">
        <a href="https://pactel.info" onclick=""> <img src="/logo.webp" width="60" height="60"
            class="justify-between dark:invert m-4" alt="logo"></a>
        <!-- <h1 style="font-weight: 800;" class="p-3 text-3xl text-gray-300">Courses</h1> -->
        <button @click="m" id="menub" class="md:hidden justify-between">
          <div class="container dark:invert px-4">
            <div class="bar1">
              <hr class="border-2 bg-black border-black">
            </div>
            <div class="bar2">
              <hr class="border-2 bg-black border-black">
            </div>
            <div class="bar3">
              <hr class="border-2 bg-black border-black">
            </div>
          </div>
        </button>
      </div>
      <div class=" flex justify-center">
        <div
          class="menu notactive bg-gray-600 text-xl font-semibold transform bg-transparent text-gray-300 transition ease-in duration-500  mt-2 px-4 bg-gray-00 "
          id="menu">
          <RouterLink to="/" @click="m"><a href="#" class="block -mb-6">Home</a></RouterLink>
          <!-- <hr class="border-1 rounded border-gray-400 m- opacity-50 "> -->
          <RouterLink to="/" @click="m" id="menub" class="block p-2">Communities</RouterLink>
          <RouterLink to="/" @click="m" id="menub" class="block p-2">The company</RouterLink>
          <RouterLink to="/" @click="m" id="menub" class="block p-2">Contact us</RouterLink>
          <a href="#" class="block p-4 mt-2 bg-orange-500 font-medium rounded-full">Get The App</a>
        </div>
      </div>
    </nav>

    <!---->
    <RouterView />
    <div class="bar h-24"></div>
    <header class=" flex justify-center space-x-10 p-2 text-white hiddenm">
      <div class="front flex mb-20">
        <div class="justify-center mr-20"><img alt="Vue logo" class="logo" src="/logo.webp" width="110" height="90" />
        </div>

        <div class="my-auto">

          <nav class="text-xl justify-center space-x-10">
            <RouterLink to="/" class="p-2">About</RouterLink>
            <RouterLink to="/about" class="p-2">Communities</RouterLink>
            <RouterLink to="/about" class="p-2">The company</RouterLink>
            <RouterLink to="/about" class="p-2">Contact us</RouterLink>
            <a href="#" class="px-5 py-2 bg-orange-500 font-medium rounded-full">Get The App</a>
          </nav>
        </div>
      </div>
    </header>


    <RouterView />
    <div class="flex-col justify-center text-5xl space-y-5 p-5 md:mt-48 mt-12 mb-48 text-center text-white font-bold">
      <p>Your Guide To</p>
      <p>Shipping Industry</p>
    </div>
    <About />
    <Features />
    <Liner />
    <Products />
    <Information />
    <Footer />
  </div>
</template>

<style scoped>
.head {
  height: 100vh;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.2)), url('/cargo.jpg') no-repeat center fixed;
  background-size: cover;

}

.bar {
  position: absolute;
  top: 0;
  width: 100%;
  backdrop-filter: blur(3px);
  -webkit-mask-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.8), transparent 100%);
}

.front {
  z-index: 9999;
  top: 0;
}

.notactive {
  text-align: center;
  z-index: 1;
  position: relative;
  overflow-y: hidden;
  width: 0vh;
  height: 0vh;
  transition: ease-in 0.6s;
}

.active {
  height: 45vh;
  width: 100%;
  background: linear-gradient(0deg, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7));
}

.bar1,
.bar2,
.bar3 {
  width: 35px;
  height: 3px;
  background-color: #0c0c0c;
  margin: 8px 5px;
  transition: 0s;
}
</style>
