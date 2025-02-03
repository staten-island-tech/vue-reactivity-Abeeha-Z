<script setup>
import "./items"

const item = defineprops("name", "price", "imageLink");
</script>

<template>
    <div v-for="item in items" :key="item.name">
    <img src=item.imageLink>    
    <h2>
        {{ item.name }}
    </h2>
    <p> {{  item.price  }}</p>
    </div>
</template>

<style scoped>
</style>



