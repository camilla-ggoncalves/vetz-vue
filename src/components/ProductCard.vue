<template>
  <div class="card">
    <img :src="img" :alt="title" />
    <h3>{{ title }}</h3>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  img: String,
});
</script>

<style scoped>
.card {
  background: white;
  border-radius: 10px;
  padding: 1rem;
  text-align: center;
  transition: transform 0.2s;
}
.card:hover {
  transform: scale(1.05);
}
.card img {
  max-width: 200px;
  margin-bottom: 1rem;
}
.card h3 {
  font-size: 1.1rem;
  font-weight: bold;
}
</style>
