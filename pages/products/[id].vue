<template>
    <div v-if="singleproduct">
        <div class="max-w-5xl mx-auto my-20">
            
            <div
                class="bg-white border rounded-xl shadow-sm sm:flex dark:bg-neutral-900 dark:border-neutral-700 dark:shadow-neutral-700/70">
                <div
                    class="shrink-0 relative w-full rounded-t-xl overflow-hidden pt-[40%] sm:rounded-s-xl sm:max-w-60 md:rounded-se-none md:max-w-xs">
                    <img :src="singleproduct.image" :alt="singleproduct.title"
                        class="size-full absolute top-0 start-0 object-cover">
                </div>
                <div class="flex flex-wrap">
                    <div class="p-4 flex flex-col h-full sm:p-7">
                        <h1 className="text-2xl font-bold text-gray-800 mb-2">{{ singleproduct.title }}</h1>
                        <p className="text-gray-600 mb-4">{{ singleproduct.description }}</p>
                        <div className="flex justify-between items-center mb-4">
                            <span className="text-lg font-semibold text-orange-600">${{ singleproduct.price }}</span>
                            <span className="text-sm text-gray-500">Category: {{ singleproduct.category }}</span>
                        </div>
                        <div className="flex items-center">
                            <span className="text-yellow-500 font-bold text-lg">
                                ⭐ {{ singleproduct.rating.rate }}
                            </span>
                            <span className="text-gray-500 text-sm ml-2">
                                ({{ singleproduct.rating.count }}reviews)
                            </span>
                        </div>
                        <div class="mt-5 sm:mt-auto">
                            <div class="px-5 mt-2 py-2.5 relative rounded group  text-white font-medium inline-block">
                                <span
                                    class="absolute top-0 left-0 w-full h-full rounded opacity-50 filter blur-sm bg-gradient-to-br from-purple-600 to-blue-500"></span>
                                <span
                                    class="h-full w-full inset-0 absolute mt-0.5 ml-0.5 bg-gradient-to-br filter group-active:opacity-0 rounded opacity-50 from-purple-600 to-blue-500"></span>
                                <span
                                    class="absolute inset-0 w-full h-full transition-all duration-200 ease-out rounded shadow-xl bg-gradient-to-br filter group-active:opacity-0 group-hover:blur-sm from-purple-600 to-blue-500"></span>
                                <span
                                    class="absolute inset-0 w-full h-full transition duration-200 ease-out rounded bg-gradient-to-br to-purple-600 from-blue-500"></span>
                                <span class="relative">Add to card</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>


    </div>
    <div v-else>
        <p>Loading product details...</p>
    </div>
</template>

<script setup>
import { useRoute } from 'vue-router'
import { ref, onMounted } from 'vue'

// Route parameter
const { id } = useRoute().params

const singleproduct = ref(null)

const fetchProduct = async () => {
    const uri = `https://fakestoreapi.com/products/${id}`
    try {
        const response = await fetch(uri)
        if (!response.ok) throw new Error('Failed to fetch product data')
        singleproduct.value = await response.json()
    } catch (error) {
        console.error(error)
    }
}

onMounted(() => {
    fetchProduct()
})
definePageMeta({
    layout: 'product'
})

</script>

<style scoped></style>