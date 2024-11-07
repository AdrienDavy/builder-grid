<template>
  <NuxtLink
    :to="`/products/${product.id}`"
    class="group bg-green-200 rounded-lg overflow-hidden cursor-pointer min-w-44 max-w-72 relative"
  >
    <div
      class="relative overflow-hidden aspect-square flex justify-center items-center bg-white"
    >
      <img
        :src="product.image"
        alt=""
        class="w-2/3 h-2/3 object-contain group-hover:scale-105 duration-300"
      />
    </div>
    <div class="p-4 flex flex-col items-center h-2/3">
      <p
        class="text-xl font-bold text-blue-500 truncate w-full pb-2"
        :title="product.title"
      >
        {{ product.title }}
      </p>
      <div
        class="text-blue-600 flex w-full flex-col text-center justify-center pb-16"
      >
        <p class="text-xl font-bold">{{ product.price }} €</p>
        <p>{{ product.rating.rate }}/5</p>
      </div>
      <button class="button absolute bottom-2">View Details</button>
    </div>
  </NuxtLink>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>
