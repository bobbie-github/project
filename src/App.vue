<script setup>

import Navbar from "./components/navbar.vue";
import Section from "./components/section.vue";
import Product from "./components/product.vue";
import Footer from "./components/footer.vue";
</script>

<template>
  <Navbar/>
  <Section/>
  <Product/>
  <Footer/>



</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
