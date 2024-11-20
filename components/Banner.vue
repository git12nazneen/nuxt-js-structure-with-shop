<template>
    <div class="relative bg-black text-white h-screen flex items-center justify-between px-10">
        <!-- Center Section -->
        <div class="absolute inset-0 flex flex-col items-center justify-center text-center z-10">
            <h1 class="text-2xl lg:text-6xl font-extrabold mb-4">Welcome to E-Shop</h1>
            <p class="text-sm lg:text-lg text-gray-300 mb-6">Discover the latest gadgets, updates, and reviews every day.</p>
            <button class="bg-red-600 text-white font-bold px-8 py-3 rounded hover:bg-red-700">
                Learn More
            </button>
        </div>
        <!-- Design Elements -->
        <div class="absolute inset-0 z-0 pointer-events-none">
            <div class="w-full h-full bg-gradient-to-r from-black via-gray-900 to-black opacity-80"></div>
            <div class="absolute left-0 top-0 w-1/2 h-1/2 bg-gradient-to-t from-red-600 to-transparent rounded-full">
            </div>
            <div
                class="absolute right-0 bottom-0 w-1/2 h-1/2 bg-gradient-to-b from-red-600 to-transparent rounded-full">
            </div>
        </div>
    </div>


</template>

<script>
export default {
    name: "Banner"
};
</script>

<style scoped>
/* Optional custom styles, you can adjust if needed */
</style>