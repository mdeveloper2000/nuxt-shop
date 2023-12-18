<template>
    <div class="container">        
        <div class="error">
            <h1>
                <LucideBan :size="42" /> Erro
            </h1>
            <h2>{{ error.message }}</h2>
            <h2>Código do erro: {{ error.statusCode }}</h2>
            <h2>Você acessou um recurso ou página que não existe ou não está disponível no momento</h2>            
            <NuxtLink :to="`/`">
                <LucideHome :size="42" />
            </NuxtLink>
        </div> 
    </div>
</template>

<script setup>
    useHead({
        title: 'Nuxt Shop | Erro'
    })
    defineProps(['error'])    
</script>

<style scoped>
    .container {
        display: flex;        
        justify-content: center;
        height: 100vh;
    }
    .error {        
        border: 1px solid  #00FA9A;
        border-radius: 8px;
        height: auto;
        padding: 30px;
        background-color: #98FB98;
        box-shadow: 4px 4px 1px 1px#00FA9A;
        align-self: center;
        text-align: center;
    }
    a {
        text-decoration: none;
        color: #000;
    }
</style>