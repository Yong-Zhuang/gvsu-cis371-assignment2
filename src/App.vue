<template>
  <header class="header">
    <!-- TODO: Write your Store Name or Add a Logo here -->
    <h1>Your Store Name</h1>
  </header>
  <nav class="nav">
    <!-- TODO: Add more navigation links if needed -->
    <a href="#" class="nav-item">Home</a>
  </nav>
  <main class="main-content">
    <!-- TODO: Use the v-for directive to list all items here using the StoreItem component -->
    <!-- Example: <StoreItem v-for="(item, index) in items" :key="index" :item="item" /> -->
  </main>
  <footer class="footer">© 2023 My Online Store. All rights reserved.</footer>
</template>

<script lang="ts" setup>
import { ref } from "vue";
import StoreItem from "./components/StoreItem.vue";

// List of products in different categories
const items = ref([
  {
    name: "Laptop",
    description: "High-end gaming laptop",
    price: 1200,
    rating: 4,
    stock: 5,
    //a fake image
    image:
      "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/wcAAwAB/sn8MOkAAAAASUVORK5CYII=",
    category: "Electronics",
  },
  // More Electronics
  {
    name: "Smartphone",
    description: "Latest model smartphone",
    price: 800,
    rating: 5,
    stock: 10,
    image:
      "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/wcAAwAB/sn8MOkAAAAASUVORK5CYII=",
    category: "Electronics",
  },
  // ... Add more electronics items ...

  // Clothing
  {
    name: "T-shirt",
    description: "100% cotton t-shirt",
    price: 20,
    rating: 4,
    stock: 25,
    image:
      "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/wcAAwAB/sn8MOkAAAAASUVORK5CYII=",
    category: "Clothing",
  },
  {
    name: "Jeans",
    description: "Slim fit jeans",
    price: 45,
    rating: 3,
    stock: 15,
    image:
      "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/wcAAwAB/sn8MOkAAAAASUVORK5CYII=",
    category: "Clothing",
  },
  // ... Add more clothing items ...

  // Groceries
  {
    name: "Apple",
    description: "Fresh red apples",
    price: 0.5,
    rating: 4,
    stock: 100,
    image:
      "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/wcAAwAB/sn8MOkAAAAASUVORK5CYII=",
    category: "Groceries",
  },
  {
    name: "Bread",
    description: "Whole grain bread",
    price: 2,
    rating: 4,
    stock: 20,
    image:
      "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/wcAAwAB/sn8MOkAAAAASUVORK5CYII=",
    category: "Groceries",
  },
  // ... Add more groceries items ...
]);
</script>

<style scoped>
/* TODO: Insert your CSS code to style the header, nav, main content, and footer */
</style>
