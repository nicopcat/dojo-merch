<template>
  <div class="card text-center">
    <img :src="products.image" alt="images" class="thumb">
    <p class="font-bold text-gray-500 m-4 truncate">{{ products.title }}</p>
    <!-- <div>{{ products.price }}</div> -->
    <a>
      <p class="btn my-4">View Detail</p>
    </a>
  </div>
</template>

<script setup>
const { products } = defineProps(['products'])
</script>

<style scoped>
.thumb {
  height: 100%;
  max-height: 120px;
  max-width: 70%;
  margin: 0 auto;
}
</style>