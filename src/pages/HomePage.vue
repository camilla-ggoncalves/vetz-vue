<template>
  <section class="home">
    <h1>A verdadeira cura começa no respeito pela vida.</h1>

    <div class="products">
      <ProductCard title="TAPETE" img="/tapete.png" />
      <ProductCard title="RAÇÃO" img="/racao.png" />
      <ProductCard title="BRINQUEDOS" img="/brinquedos.png" />
      <ProductCard title="CAMA" img="/cama.png" />
    </div>
  </section>
</template>

<script setup>
import ProductCard from "../components/ProductCard.vue";
import { useRouter } from 'vue-router';

const router = useRouter();

const goToProducts = () => {
  router.push('/products');
}

const goToAbout = () => {
  router.push('/about');
}
</script>

<style scoped>
.home {
  padding: 2rem;
  text-align: center;
}
.home h1 {
  font-size: 2rem;
  font-weight: bold;
  color: #008000;
  margin-bottom: 2rem;
}
.products {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 2rem;
  justify-items: center;
}
</style>
