<template>
    <div>
       
        <p>prodct details for {{  id }}</p>
        <p>
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Amet accusantium modi odit atque doloribus 
            repudiandae officiis fugiat magni. Rem distinctio pariatur adipisci, cumque reiciendis fugiat cum 
            voluptas voluptatem natus deserunt.
        </p>
    </div>
</template>

<script setup>
    const {id} = useRoute().params

    definePageMeta({
        layout:'products'
    });


    //https://tailwindcss.nuxtjs.org/getting-started/setup
    //to add tailwind css to nuxt project
</script>

