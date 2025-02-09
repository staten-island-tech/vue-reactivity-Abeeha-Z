<script setup>
const cart_items = []
</script>

<template>
  <div v-for="cart_item in cart_items" :key="cart_item.id"></div>
</template>

<style scoped></style>
