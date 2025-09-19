<script setup>
import NavComponent from '../src/components/NavComponent.vue';
import Footer from "./components/Footer.vue"; // importa o rodapé
</script>

<template>
  <NavComponent></NavComponent>

  <router-link to="/home">Homepage</router-link>
  <router-link to="/about">Sobre Nós</router-link>

  <router-view /> <!-- Para aparecer o conteúdo das páginas -->

  <Footer />
</template>

<style scoped>
</style>
