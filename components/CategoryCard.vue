<template>
    <div class="card">
        <div class="card-body">
            <!-- <img :src="product.image" class="card-image"> -->
        </div>
        <div class="card-header">
           <!-- <NuxtLink :to="`products/${product.id}`">See Details</NuxtLink> -->
        </div>
    </div>
</template>

<script setup>
const {product} = defineProps(["product"]);
</script>

<style lang="scss" scoped>

</style>