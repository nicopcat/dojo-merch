<template>
  <div>
    <header class="shadow-sm bg-whie">
      <nav class="container mx-auto p-4">
        <NuxtLink to="/" class="font-bold ">Dojo Merch</NuxtLink>
      </nav>
    </header>

    <!-- output the page content -->
    <div class="container mx-auto p-4">
      <slot />
    </div>

    <footer class="container mx-auto p-4 flex justify-between border-t-2">
      <ul class="flex gap-5">
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/products">Products</NuxtLink>
        </li>
      </ul>

    </footer>
  </div>
</template>

<script setup>

</script>

<style scoped>
.router-link-exact-active {
  color: #12b444
}
</style>