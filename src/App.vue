<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Titan from './components/Titan.vue'
import Header from './components/Header.vue'
import ProductList from './components/catalog/ProductList.vue'
</script>

<template>
  <Header />
  <main class="wrapper">
    <ProductList />
  </main>
  <!-- <Titan /> -->
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
