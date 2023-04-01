<template>
        <div class="card">
            <img :src="product.image" class="card-image">
            <NuxtLink :to="`/${product.id}`" class="btn">See Details</NuxtLink>
        </div>
</template>

<script setup>
const {product} = defineProps(["product"]);
</script>
