<template>
    <div>
        <h1>Products details {{ id }}</h1>
    </div>
</template>

<script setup>
const { id } = useRoute().params
definePageMeta({
    layout: 'product'
})

</script>

<style scoped></style>