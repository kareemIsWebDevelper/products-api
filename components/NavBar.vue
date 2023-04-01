<template>
    <header>
        <nav class="navbar">
            <div class="container-fluid">
                <NuxtLink to="/" class="nav-link" id="navbar-brand">
                <span>S</span><p>TORE</p>
                </NuxtLink>
                <NuxtLink to="/products" class="nav-link">
                    Products
                </NuxtLink>
                <div class="nav">
                    <div id="dropdown">
                        <h3 id="dropdown-link">
                            Category
                        </h3>
                        <div id="dropdown-menu">
                            <!-- <NuxtLink to="/electro">electronics</NuxtLink>
                            <NuxtLink to="/jewellary">jewelery</NuxtLink>
                            <NuxtLink to="/men">men's clothing</NuxtLink>
                            <NuxtLink to="/women">women's clothing</NuxtLink> -->
                        </div>
                    </div>
                </div>
            </div>
        </nav>
    </header>
</template>

<script setup>
const CategoryApi = "https://fakestoreapi.com/products/categories";
const { data: categories } = useFetch(CategoryApi);
</script>

<style scoped>
@import url("../assets/nav.css");
</style>