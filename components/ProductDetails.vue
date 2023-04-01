<template>
    <div class="card">
        <div class="card-body">
            <img :src="product.image" class="card-image">
        </div>
        <div class="card-header">
            <div class="flex-header">
                <h2>{{ product.title }}</h2>
                <h1>{{ product.price }}$</h1>
            </div>
            <div class="flex-description">
                <p>{{ product.description }}</p>
            </div>
        </div>
    </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>

<style scoped>
    .card {
        display: flex;
        /* width: 70%; */
        justify-content: space-around;
        width: 70%;
        gap: 50px;
        justify-content: center;
        margin-left: 200px;
        margin-top: 50px;
    }

    .flex-header {
       display: grid;
       margin-top: 150px;
        gap: 20px;
    }
    .card-image {
        width: 400px;
        height: 500px;
    }
</style>