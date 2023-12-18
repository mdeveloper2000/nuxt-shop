<template>
    <HeaderCard />
    <Menu />
    <div class="container">
        <slot />
    </div>        
</template>

<style scoped>
    .container {
        display: flex;
        height: 100vh;        
        flex-flow: row wrap;
        justify-content: center;
    }
</style>