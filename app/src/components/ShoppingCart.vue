<script setup>
const props = defineProps({
  cart_items: {
    type: Array,
    required: true,
  },
})

function calcTotal() {
  return props.cart_items.reduce((total, cart_item) => total + cart_item.price, 0)
}
</script>

<template>
  <div class="fixed right-0 top-0 w-80 h-screen bg-gray-100 border-l border-gray-300 p-4">
    <h2 class="text-xl font-semibold mb-4">Shopping Cart</h2>

    <div
      v-for="cart_item in cart_items"
      :key="cart_item.name"
      class="mb-2 flex justify-between items-center border-b py-2"
    >
      <span class="text-sm font-medium">{{ cart_item.name }}</span>
      <span class="text-sm text-gray-500">${{ cart_item.price }}</span>
    </div>

    <div class="mt-4 flex justify-between font-semibold text-lg">
      <span>Total:</span>
      <span>${{ calcTotal() }}</span>
    </div>
  </div>
</template>
