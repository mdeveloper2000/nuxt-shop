<template>
    <header>
        <nav>
            <ul>
                <li>
                    <NuxtLink to="/">
                        <LucideHome /> Home
                    </NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/products">
                        <LucideShoppingBasket />Produtos
                    </NuxtLink>
                </li>
                <li>
                    <NuxtLink to="/about">
                        <LucideInfo /> Sobre
                    </NuxtLink>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
    ul {
        list-style-type: none;
        margin: 0;
        padding: 0;
        overflow: hidden;
        border: 2px solid #04AA6D;
        background-color: #fff;
    }
    li {
        float: left;
    }
    li a {
        display: block;
        color: #000;
        font-size: 18px;  
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
    }
    li a:hover:not(.router-link-exact-active) {
        background-color: #04AA6D;
        color: #fff;
    }
    li .router-link-exact-active {
        color: #fff;
        background-color: #04AA6D;
    }
</style>