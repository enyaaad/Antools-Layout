<script setup lang="ts">
import HeaderComponent from "./components/header.vue";
import Layout from "./components/layout.vue";
import FooterComponent from "./components/footer.vue";
</script>

<template>
  <header-component></header-component>
  <layout></layout>
  <footer-component></footer-component>
</template>

<style scoped>
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
