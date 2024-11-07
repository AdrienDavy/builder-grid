<template>
  <header>
    <nav class="flex bg-gray-500">
      <NuxtLink
        to="/"
        class="bg-gray-400 text-center text-green-200 hover:text-green-400 transition-all duration-300 font-bold text-2xl p-4 text-nowrap"
        >Builder Grid</NuxtLink
      >
      <ul
        class="flex justify-evenly w-full text-green-400 font-bold text-xl items-center"
      >
        <li>
          <NuxtLink
            to="/"
            class="hover:text-green-500 transition-all duration-300"
            active-class="text-blue-300 underline"
            >Home</NuxtLink
          >
        </li>
        <li>
          <NuxtLink
            to="/about"
            class="hover:text-green-500 transition-all duration-300"
            active-class="text-blue-300 underline"
            >About</NuxtLink
          >
        </li>
        <li>
          <NuxtLink
            to="/products"
            class="hover:text-green-500 transition-all duration-300"
            active-class="text-blue-300 underline"
            >Products</NuxtLink
          >
        </li>
      </ul>
    </nav>
  </header>
  <main>
    <slot />
  </main>
</template>
