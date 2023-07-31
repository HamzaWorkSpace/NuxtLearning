<template>
    <div>
        <ProductDetail :productDetail="product"/> 

    </div>
</template>

<script setup>
    const {id} = useRoute().params;

    const uri = 'https://fakestoreapi.com/products/'+id;

    const {data:product} = await useFetch(uri,{key:id});

    definePageMeta({
        layout:'products'
    });

    //console.log(product);

    //https://tailwindcss.nuxtjs.org/getting-started/setup
    //to add tailwind css to nuxt project
</script>

