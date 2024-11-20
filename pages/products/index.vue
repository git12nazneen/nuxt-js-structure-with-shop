<template>
    <div class="container mx-auto p-10">
        <Heading title="See Our all Product" subTitle="Our all products are authentic and new available"></Heading>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5 my-10">
            <div v-for="product in products">
                <a
                    class="flex flex-col bg-white border shadow-sm rounded-xl hover:shadow-lg focus:outline-none focus:shadow-lg transition dark:bg-neutral-900 dark:border-neutral-700 dark:shadow-neutral-700/70 h-[480px]">

                    <img :src="product.image" :alt="product.title" class="w-full h-72 p-7 rounded-t-xl" />
                    <div class="p-4 md:p-5">
                        <h3 class="text-lg font-bold text-gray-800 dark:text-white">
                            {{ product.title.slice(0, 20) }}
                        </h3>
                        <p class="mt-1 text-gray-500 dark:text-neutral-400">
                            {{ product.description.slice(0, 110) }}
                        </p>
                        <button>
                            <NuxtLink :to="`/products/${product.id}`">
                                <Gbutton> See Details</Gbutton>
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