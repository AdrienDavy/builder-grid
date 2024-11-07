<script setup lang="ts">
const route = useRoute();
</script>

<template>
  <div>
    <h1 class="text-green-400 font-bold text-center text-5xl">Home</h1>
    <p>
      Current route:
      <strong class="text-purple-500">{{ route.name }} </strong> which url is
      <strong class="text-purple-500">{{ route.path }}</strong>
    </p>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusantium
      numquam temporibus hic dolorum deserunt praesentium pariatur provident
      rerum velit?
    </p>
  </div>
</template>
