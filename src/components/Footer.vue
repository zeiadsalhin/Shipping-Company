<script setup>
</script>
<template>
    <div class="footer flex-col justify-center text-center p-5 mx-auto mt-20">
        <h1 class="text-4xl font-extrabold text-white p-5">Get your Quote</h1>
        <p class="text-gray-100 text-xl font-semibold">FREE Quotes for New Customers NOW</p>
        <div class="qoute p-10 space-x-10 flex justify-center">
            <button class="px-5 py-3 rounded-xl text-orange-700 text-xl bg-orange-200">Call us</button>
            <button class="px-5 py-3 rounded-xl text-white text-xl bg-orange-700">Email Us</button>
        </div>
        <img class="p-2 brightness-100 mx-auto" width="100" height="" src="/logo.webp" alt="">
        <div class="text md:flex justify-center space-x-10 p-5">
            <button class="text-white hover:bg-transparent hover:text-orange-500">Overview</button>
            <button class="text-white hover:bg-transparent hover:text-orange-500">Features</button>
            <button class="text-white hover:bg-transparent hover:text-orange-500">Pricing</button>
            <button class="text-white hover:bg-transparent hover:text-orange-500">Quotes</button>
            <button class="text-white hover:bg-transparent hover:text-orange-500">Help</button>
            <button class="text-white hover:bg-transparent hover:text-orange-500">FAQ</button>
        </div>
        <div class="credits flex-col space-y-3 justify-center p-5">
            <img class="bg-white rounded-full mx-auto p-1 m-2 hover:bg-orange-500" width="40" height=""
                src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg">
            <a href="https://github.com/zeiadsalhin"
                class="text-gray-100 hover:bg-transparent hover:text-orange-600">Credits: Created By Ziad</a>
        </div>
    </div>
</template>
<style>
.footer {
    height: 90vh;
    background: linear-gradient(0deg, rgba(0, 0, 0, 2), rgba(0, 0, 0, 0.1)), url('/cargo.jpg') no-repeat center fixed;
    background-size: cover;
}
</style>