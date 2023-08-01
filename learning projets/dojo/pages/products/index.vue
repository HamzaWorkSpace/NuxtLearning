<template>
    <div> 
        <Head>
            <Title>Nuxt Dojo | products</Title>
            <Meta name='description' content="Nuxt 3 products page"/>
        </Head> 
        <div class ="grid grid-cols-5 gap-5">
            <!-- looping through the products and assigning product ID to the URL -->
            <div v-for="p in products">
                <ProductCard :productData="p"/>
            </div>
        </div>      
    </div>
</template>

<script setup>

    //defining layout of the page
    definePageMeta({
        layout:'products'
    });

    //fetch data and name the data as products
    const {data:products} = await useFetch('https://fakestoreapi.com/products');


    // useHead({
    //     title: 'Nuxt Dojo | products',
    //     meta:[
    //         {
    //             name: 'description',
    //             content: 'Nuxt 3 products page'
    //         }
    //     ]
    // })

</script>

<style scoped>

h2{
    margin-bottom: 20px;
    font-size: 36px;
}
p{
    margin:20px 0;
}

</style>