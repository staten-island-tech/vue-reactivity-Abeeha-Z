<script setup>
import items from './items'
import ShoppingCart from './ShoppingCart.vue'
import { ref } from 'vue'

const cart_items = ref([])

function add_toCart(item) {
  cart_items.value.push(item)
}
</script>

<template>
  <div class="flex flex-wrap m-5 p-2 w-4/5 h-auto">
    <div
      class="w-60 text-lg text-wrap border-gray-300 border-2 m-2 p-2 text-center bg-red-100"
      v-for="item in items"
      :key="item.name"
    >
      <img :src="item.imageLink" class="h-60 w-60 m-bottom-2" />
      <h2>
        {{ item.name }}
      </h2>
      <p>${{ item.price.toFixed(2) }}</p>
      <button class="rounded p-2 m-2 text-sm border-black border-1" @click="add_toCart(item)">
        Add to Cart
      </button>
    </div>
  </div>
  <ShoppingCart :cart_items="cart_items" />
</template>

<style scoped></style>
