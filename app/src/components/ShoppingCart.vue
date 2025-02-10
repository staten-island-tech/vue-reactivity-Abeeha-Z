<script setup>
const cart_items = []
function calcTotal(cart_item) {
  total_price = 0
  cart_items.forEach((cart_item)=> total_price.add(cart-items.price))
}
  console.log(total_price);
  return total_price
</script>

<template>
  <div v-for="cart_item in cart_items" :key="cart_item.id" :cart_item="cart_item">
    <div class="inline-flex">
      <h1>{{cart_item.name}} ------ </h1>
      <p>{{ cart_item.price }}</p>
    </div>

  </div>
</template>

<style scoped></style>
