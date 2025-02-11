<script setup>
import items from './items'
import ShoppingCart from './ShoppingCart.vue';
</script>

<template>
  <div class="flex flex-wrap m-2 p-2 w-full h-auto">
    <div class="w-48 text-wrap border-black border-2 m-3 p-3" v-for="item in items" :key="item.name">
      <img :src="item.imageLink" class="w-32 h-48" />
      <h2>
        {{ item.name }}
      </h2>
      <p>${{ item.price }}</p>
      <button class="border-black border-1" @click="add_toCart(item)">Add to Cart</button>
    </div>
  </div>
</template>

<style scoped></style>
