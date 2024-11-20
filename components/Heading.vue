<template>
    <div class="text-center my-6">
        <h1 class="text-xl lg:text-6xl font-bold text-gray-800">
            {{ title }}
        </h1>
        <h2 class="text-sm lg:text-xl font-light text-gray-800">
            {{ subTitle }}
        </h2>
    </div>
</template>

<script>
export default {
  name: "Heading",
  props: {
    title: {
      type: String,
      required: true,
    },
    subTitle: {
      type: String,
      required: true,
    },
  },
};
</script>

