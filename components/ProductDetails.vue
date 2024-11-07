<template>
  <div class="flex justify-center w-full">
    <div class="bg-green-200 overflow-hidden w-full">
      <div
        class="relative overflow-hidden w-full bg-white flex justify-center p-8"
      >
        <img :src="product.image" alt="" class="w-80 h-80 object-contain" />
      </div>
      <div class="p-4">
        <p
          class="text-xl font-bold text-blue-500 truncate"
          :title="product.title"
        >
          {{ product.title }}
        </p>
        <p class="text-lg text-blue-500 truncate pb-8">
          {{ product.category }}
        </p>
        <div class="text-blue-600 flex w-full justify-between pb-8">
          <p class="text-2xl">{{ product.price }} €</p>
          <p>{{ product.rating.rate }}/5</p>
        </div>
        <p class="text-blue-600 text-xs">{{ product.description }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>
