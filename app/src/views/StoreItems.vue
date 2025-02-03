
<template>
    <div>    
    <li v-for="item in items">
        {{ createCards() }}
    </li>
    </div>
</template>


<style scoped>
</style>

<script setup>

const items = [
  {
    name: "Croissant",
    price: 2.50,
    imageLink: "https://www.example.com/croissant.jpg"
  },
  {
    name: "Chocolate Chip Cookie",
    price: 1.75,
    imageLink: "https://www.example.com/chocolate-chip-cookie.jpg"
  },
  {
    name: "Cinnamon Roll",
    price: 3.00,
    imageLink: "https://www.example.com/cinnamon-roll.jpg"
  },
  {
    name: "Brioche Bun",
    price: 2.00,
    imageLink: "https://www.example.com/brioche-bun.jpg"
  },
  {
    name: "Lemon Pound Cake",
    price: 4.50,
    imageLink: "https://www.example.com/lemon-pound-cake.jpg"
  },
  {
    name: "Sourdough Bread",
    price: 5.00,
    imageLink: "https://www.example.com/sourdough-bread.jpg"
  },
  {
    name: "Apple Turnover",
    price: 3.25,
    imageLink: "https://www.example.com/apple-turnover.jpg"
  },
  {
    name: "Blueberry Muffin",
    price: 2.75,
    imageLink: "https://www.example.com/blueberry-muffin.jpg"
  },
  {
    name: "Vanilla Cupcake",
    price: 2.00,
    imageLink: "https://www.example.com/vanilla-cupcake.jpg"
  },
  {
    name: "Raisin Scone",
    price: 3.50,
    imageLink: "https://www.example.com/raisin-scone.jpg"
  },
  {
    name: "Pecan Pie",
    price: 5.00,
    imageLink: "https://www.example.com/pecan-pie.jpg"
  },
  {
    name: "Chocolate Éclair",
    price: 3.25,
    imageLink: "https://www.example.com/chocolate-eclair.jpg"
  },
  {
    name: "Almond Croissant",
    price: 3.50,
    imageLink: "https://www.example.com/almond-croissant.jpg"
  },
  {
    name: "Pumpkin Spice Muffin",
    price: 3.00,
    imageLink: "https://www.example.com/pumpkin-spice-muffin.jpg"
  }
];
</script>
