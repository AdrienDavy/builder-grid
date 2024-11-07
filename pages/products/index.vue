<template>
  <div class="flex flex-wrap gap-4 p-8 justify-center">
    <ProductCard
      v-for="product of products"
      :key="product.id"
      :product="product"
    />
  </div>
</template>
<script setup>
definePageMeta({
  layout: "products",
});
const { data: products } = await useFetch("https://fakestoreapi.com/products");
console.log(products.value);
</script>
