<template>
    <div class="myCard">
        <div v-for="product in products" :key="product.id">
            <ProductCard :product="product"/>
        </div>
    </div>
</template>

<script setup>
const { data: products } = useFetch("https://fakestoreapi.com/products");

definePageMeta({
    layout: "products"
})
</script>

<style scoped></style>