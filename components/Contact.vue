<template>
    <div>
        <div class="  px-6 md:px-16">
  <div class="max-w-6xl mx-auto">
    <!-- Title -->
   <Heading title="Contact us" subTitle='Start with us..'></Heading> 
    <div class="grid md:grid-cols-2 gap-8 py-10">
      <!-- Card 1 -->
      <div class="bg-white rounded-lg shadow-lg p-6 text-center">
        <div class="flex justify-center mb-4">
          <img src="https://images.pexels.com/photos/11798029/pexels-photo-11798029.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Icon" class="w-20 h-20 rounded-full">
        </div>
        <h2 class="text-lg font-semibold text-gray-800 mb-2">Talk to a member of our Sales team</h2>
        <p class="text-sm text-gray-600 mb-6">
          We’ll help you find the right products and pricing for your business.
        </p>
        
        <Gbutton>     Contact Sales </Gbutton>
      </div>
      
      <!-- Card 2 -->
      <div class="bg-white rounded-lg shadow-lg p-6 text-center">
        <div class="flex justify-center mb-4">
          <img src="https://images.pexels.com/photos/8817532/pexels-photo-8817532.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" alt="Icon" class="w-20 h-20 rounded-full">
        </div>
        <h2 class="text-lg font-semibold text-gray-800 mb-2">Product and account support</h2>
        <p class="text-sm text-gray-600 mb-6">
          Our help center is fresh and always open for business. If you can’t find the answer you’re looking for, we’re here to lend a hand.
        </p>
        <Gbutton>  Go to the help center</Gbutton>
      </div>
    </div>
  </div>
</div>

    </div>
</template>

<script>
    export default{
         name: "Contact"
    }
</script>

<style lang="scss" scoped>

</style>