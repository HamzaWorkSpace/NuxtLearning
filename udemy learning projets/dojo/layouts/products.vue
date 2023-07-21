<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4">
                <NuxtLink to="/products" class="font-bold" >Dojo Products</NuxtLink>
               
            </nav>
        </header>
    </div>
    <!--output the content page-->
    <div class="container mx-auto p-4">
        <slot />
    </div>
    <footer class="container mx-auto p-4 justify-between border-t-2">
        <ul class="flex gap-4">
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/about">about</NuxtLink></li>
            <li><NuxtLink to="/products">products</NuxtLink></li>
        </ul>
    </footer>
</template>

<style scoped>
.router-link-exact-active{
    color:#12b488;
}
</style>

