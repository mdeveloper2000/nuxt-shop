<template>
    <div class="about">
        <h1>Sobre</h1>
        <h3>Nuxt Shop (simulador de loja virtual)</h3>
        <h4>App desenvolvido para aprimorar os conhecimentos no Framework Nuxt</h4>
    </div>    
</template>

<script setup>
    useHead({
        title: 'Nuxt Shop | Sobre'
    })
</script>

<style>
    .about {
        border: 1px solid  #00FA9A;
        border-radius: 8px;
        height: auto;
        padding: 30px;
        background-color: #98FB98;
        box-shadow: 4px 4px 1px 1px #00FA9A;
        align-self: flex-start;
        margin-top: 100px;
    }
</style>