<template>
    <div class="container mx-auto p-10">
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5">
            <div v-for="product in products">
                <a class="flex flex-col bg-white border shadow-sm rounded-xl hover:shadow-lg focus:outline-none focus:shadow-lg transition dark:bg-neutral-900 dark:border-neutral-700 dark:shadow-neutral-700/70 h-[440px]"
                    >
                    <img class="w-full h-auto rounded-t-xl"
                        src="https://images.unsplash.com/photo-1680868543815-b8666dba60f7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=320&q=80"
                        alt="Card Image">
                    <div class="p-4 md:p-5">
                        <h3 class="text-lg font-bold text-gray-800 dark:text-white">
                           {{ product.title.slice(0,20) }}
                        </h3>
                        <p class="mt-1 text-gray-500 dark:text-neutral-400">
                           {{ product.description.slice(0,160) }}
                        </p>
                        <button>
                            <NuxtLink :to="`/products/${product.id}`">
                                <a href="#_" class="px-5 mt-2 py-2.5 relative rounded group font-medium text-white font-medium inline-block">
    <span class="absolute top-0 left-0 w-full h-full rounded opacity-50 filter blur-sm bg-gradient-to-br from-purple-600 to-blue-500"></span>
    <span class="h-full w-full inset-0 absolute mt-0.5 ml-0.5 bg-gradient-to-br filter group-active:opacity-0 rounded opacity-50 from-purple-600 to-blue-500"></span>
    <span class="absolute inset-0 w-full h-full transition-all duration-200 ease-out rounded shadow-xl bg-gradient-to-br filter group-active:opacity-0 group-hover:blur-sm from-purple-600 to-blue-500"></span>
    <span class="absolute inset-0 w-full h-full transition duration-200 ease-out rounded bg-gradient-to-br to-purple-600 from-blue-500"></span>
    <span class="relative">See Details</span>
</a>
                            </NuxtLink>
                        </button>
                    </div>
                </a>
            </div>
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: 'product'
})

// fetch the data
const { data: products } = await useFetch('https://fakestoreapi.com/products')

</script>

<style scoped></style>