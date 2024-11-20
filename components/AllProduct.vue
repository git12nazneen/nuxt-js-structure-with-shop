<template>
    <Heading title="See Our all Product" subTitle="Our all products are authentic and new available"></Heading>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5 my-10 container mx-auto">

        <div class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden">
            <!-- Top Section -->
            <div class="relative bg-black h-40 flex items-center justify-center">
                <h1 class="text-4xl font-bold text-white uppercase text-center">Walk in<br />Confidence</h1>
            </div>

            <!-- Middle Section: Image and Discount -->
            <div class="relative -mt-12 flex justify-center items-center">
                <img src="https://fakestoreapi.com/img/81fPKd-2AYL._AC_SL1500_.jpg" alt="Shoes"
                    class="w-40 h-auto object-cover z-10">
                <div class="absolute top-4 right-4 bg-black text-white text-center rounded-full p-4">
                    <p class="text-lg font-bold">40%</p>
                    <p class="text-sm uppercase">Off</p>
                </div>
            </div>

            <!-- Bottom Section: Description -->
            <div class="p-6 text-center">
                <p class="text-gray-600 text-sm">
                    Experience ultimate comfort with our new arrival shoes. Engineered with the latest technology for
                    superior support and cushioning. Elevate your look and make a statement wherever you go.
                </p>
            </div>
        </div>
        <div class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden">
            <!-- Top Section -->
            <div class="relative bg-black h-40 flex items-center justify-center">
                <h1 class="text-4xl font-bold text-white uppercase text-center">Walk in<br />Confidence</h1>
            </div>

            <!-- Middle Section: Image and Discount -->
            <div class="relative -mt-12 flex justify-center items-center">
                <img src="https://fakestoreapi.com/img/71li-ujtlUL._AC_UX679_.jpg" alt="Shoes"
                    class="w-40 h-auto object-cover z-10">
                <div class="absolute top-4 right-4 bg-black text-white text-center rounded-full p-4">
                    <p class="text-lg font-bold">40%</p>
                    <p class="text-sm uppercase">Off</p>
                </div>
            </div>

            <!-- Bottom Section: Description -->
            <div class="p-6 text-center">
                <p class="text-gray-600 text-sm">
                    Experience ultimate comfort with our new arrival shoes. Engineered with the latest technology for
                    superior support and cushioning. Elevate your look and make a statement wherever you go.
                </p>
            </div>
        </div>
        <div class="max-w-sm mx-auto bg-white shadow-lg rounded-lg overflow-hidden">
            <!-- Top Section -->
            <div class="relative bg-black h-40 flex items-center justify-center">
                <h1 class="text-4xl font-bold text-white uppercase text-center">Walk in<br />Confidence</h1>
            </div>

            <!-- Middle Section: Image and Discount -->
            <div class="relative -mt-12 flex justify-center items-center">
                <img src="https://fakestoreapi.com/img/61U7T1koQqL._AC_SX679_.jpg" alt="Shoes"
                    class="w-40 h-auto object-cover z-10">
                <div class="absolute top-4 right-4 bg-black text-white text-center rounded-full p-4">
                    <p class="text-lg font-bold">40%</p>
                    <p class="text-sm uppercase">Off</p>
                </div>
            </div>

            <!-- Bottom Section: Description -->
            <div class="p-6 text-center">
                <p class="text-gray-600 text-sm">
                    Experience ultimate comfort with our new arrival shoes. Engineered with the latest technology for
                    superior support and cushioning. Elevate your look and make a statement wherever you go.
                </p>
            </div>
        </div>



    </div>
    <div class="flex items-center justify-center py-10 mx-auto">
        <NuxtLink to="/products">
            <Gbutton>See All Products</Gbutton>
        </NuxtLink>
    </div>

</template>

<script>
export default {
    name: "AllProduct"
};
</script>

<style lang="scss" scoped></style>