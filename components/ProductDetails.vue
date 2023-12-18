<template>
    <div class="container">
        <div class="detail">
            <h1>{{ product.title }}</h1>
            <img :src="product.image" />
            <h2>{{ product.description }}</h2>
            <h2>Preço: ${{ product.price }}</h2>
            <NuxtLink class="btn">
                <LucideShoppingCart /> Adicionar ao carrinho
            </NuxtLink>    
        </div>
        <div class="links">
            <NuxtLink :to="`/`">
                <LucideHome :size="48" />
            </NuxtLink>
            <NuxtLink :to="`/products`">
                <LucideUndo2 :size="48" />
            </NuxtLink>            
        </div>        
    </div>  
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>

<style scoped>
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 50%;
    }
    .detail {        
        margin-top: 15px;        
        padding: 50px;
        border: 2px solid #00FA9A;
        text-align: center;
        border-radius: 8px;        
    }
    .btn {
        width: 80%;
        padding: 20px;
        margin-top: 20px;
        background-color: #00FA9A;
        border-radius: 8px;
    }
    a {
        text-decoration: none;
        color: #000;
    }
    .links {
        margin-top: 50px;
        margin-bottom: 50px;        
    }
    .links a {
        margin-left: 50px;
        margin-right: 50px;
    }
</style>