<template>
  <div>
    <div class="grid grid-cols-4 gap-4">
      <div v-for="p in products" @click="detail(p)">
        <ProductCard :products="p" />
      </div>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: 'products'
})

const uri = 'https://fakestoreapi.com/products';
const { data: products } = await useFetch(uri);
const router = useRouter();

function detail(p) {
  router.push({ path: `/products/${p.id}` });
}
</script>

<style scoped></style>