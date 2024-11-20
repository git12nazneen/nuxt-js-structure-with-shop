<template>
  <div class="px-5 mt-2 py-2.5 relative rounded group text-white font-medium inline-block">
    <span
      class="absolute top-0 left-0 w-full h-full rounded opacity-50 filter blur-sm bg-gradient-to-br from-[#a01d1f] to-black"></span>
    <span
      class="h-full w-full inset-0 absolute mt-0.5 ml-0.5 bg-gradient-to-br filter group-active:opacity-0 rounded opacity-50 from-[#a01d1f] to-black"></span>
    <span
      class="absolute inset-0 w-full h-full transition-all duration-200 ease-out rounded shadow-xl bg-gradient-to-br filter group-active:opacity-0 group-hover:blur-sm from-[#a01d1f] to-black"></span>
    <span
      class="absolute inset-0 w-full h-full transition duration-200 ease-out rounded bg-gradient-to-br to-[#a01d1f] from-black"></span>
    <span class="relative">
      <slot>See Details</slot>
    </span>
  </div>
</template>

<script>
export default {
  name: "Gbutton",
};
</script>