<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink to="/" class="font-bold">Dojo</NuxtLink>
                <ul class="flex gap-4">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">about</NuxtLink></li>
                    <li><NuxtLink to="/products" class="btn">products</NuxtLink></li>
                    <li><NuxtLink to="/products/hamza">hamza</NuxtLink></li>
                </ul>
            </nav>
        </header>
    </div>
    <!--output the content page-->
    <div class="container mx-auto p-4">
        <slot />
    </div>
</template>



<style scoped>
.router-link-exact-active{
    color:#12b488;
}
</style>