<template>
    <div class="card test-center">
        <img :src="productData.image" alt="product thumb" class="thumb">
        <p class="font-bold text-gray-500 m-4 truncate">{{ productData.title }}</p>
        <NuxtLink :to="`/products/${productData.id}`">
        <p class="btn my-4">View Details</p>
        </NuxtLink>
    </div>
</template>

<script setup>

    const {productData} = defineProps([
        'productData'
    ])

</script>

<style scoped>

.thumb{
    max-height:120px;
    max-width:70%;
    margin: 0 auto;
}

</style>