<template>
    <NuxtLink :to="`/products/${product.id}`">
        <div class="item">
            <img :src="product.image" alt="product image" />
            <h4>{{ product.title }}</h4>
            <NuxtLink :to="`/products/${product.id}`" class="btn">
                <LucideMousePointerSquare /> Clique para ver detalhes                
            </NuxtLink>
        </div>
    </NuxtLink>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
    .item {
        display: flex;
        flex-direction: column;
        margin: 20px;
        border: 2px solid #00FA9A;
        padding: 10px;
        border-radius: 8px;
        height: 400px;
        width: 260px;
        align-items: center;
        justify-content: space-between;
    }
    a {
        text-decoration: none;
        color: #000;
    }
    img {
        width: 200px;
        height: 250px;
    }
    .btn {
        width: 75%;
        padding: 10px;        
        background-color: #00FA9A;
        border-radius: 8px;
    }
</style>