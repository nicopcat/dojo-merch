<template>
  <div class="card ">
    <div class="grid grid-cols-2 gap-10">
      <div>
        <img :src="product.image" alt="images" class="mx-auto my-10">
      </div>
      <div class="p-7">
        <h2 class="text-2xl my-7">{{ product.title }}</h2>
        <p class="text-xl my-7">Price - ${{ product.price }}</p>
        <p class="font-bold border-b-2 mb-4 pb-2 my-7">Description: </p>
        <p class="mb-7">{{ product.description }}</p>
      </div>

    </div>
  </div>
</template>

<script setup>
const { product } = defineProps(['product'])
</script>

<style scoped></style>