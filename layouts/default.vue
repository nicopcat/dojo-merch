<template>
  <div>
    <header class="shadow-sm bg-whie">
      <nav class="container mx-auto p-4 flex justify-between">
        <NuxtLink to="/" class="font-bold ">Dojo Merch</NuxtLink>
        <ul class="flex gap-4">
          <li>
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/products" class="btn">Products</NuxtLink>
          </li>
        </ul>

      </nav>
    </header>

    <!-- output the page content -->
    <div class="container mx-auto p-4">
      <slot />
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.router-link-exact-active {
  color: #12b444
}
</style>