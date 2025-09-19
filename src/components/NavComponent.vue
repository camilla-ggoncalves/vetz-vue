<template>
  <header class="header">
    <nav class="navbar navbar-default navbar-fixed-top">
      <div class="container">
        <nav class="navbar navbar-expand-lg">

          <!-- Logo -->
          <RouterLink to="/" rel="home">
            <img
              class="logomenu"
              src="../assets/logo-vetz.svg"
              alt="VET Z"
              title="VetZ"
            />
          </RouterLink>

          <!-- Botão hamburger -->
          <button
            class="navbar-toggler collapsed"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarCollapse"
            aria-controls="navbarCollapse"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon">
              <i class="fas fa-bars"></i>
            </span>
          </button>

          <!-- Menu -->
          <div class="navbar-collapse collapse" id="navbarCollapse">
            <ul class="navbar-nav ml-auto left-menu">
              <li><RouterLink to="/home">HOME PAGE</RouterLink></li>
              <li><RouterLink to="/about">SOBRE NÓS</RouterLink></li>
              <li>CURIOSIDADES</li>
              <li>RECOMENDAÇÕES</li>
              <li>VACINAÇÃO</li>
              <li>CADASTRAR</li>
            </ul>
          </div>

        </nav>
      </div>
    </nav>
  </header>
</template>

<script setup>
import { RouterLink } from 'vue-router';
</script>

<style scoped>
.navbar {
  width: 100%;
  z-index: 9999;
  padding: 4px 0;
  background-color: #FEFFEF;
  box-shadow: 0px 0px 25px 0px #2125295c;
}

.navbar-brand {
  font-family: 'Arial, Helvetica, sans-serif';
  font-size: 28px;
  font-weight: 100;
  color: #000 !important;
}

.navbar-toggler {
  padding: 5px 10px;
  font-size: 24px;
  line-height: 1;
  background-color: transparent;
  border-radius: 6px;
  border: 1px solid #FEFFEF;
}

.navbar-toggler-icon i {
  color: #000;
}

.navbar-fixed-top .navbar-nav > li > a {
  color: #000 !important;
  font-size: 16px;
  line-height: 1;
  padding: 10px 15px;
  font-family: 'Arial, Helvetica, sans-serif';
  font-weight: 100;
  letter-spacing: 1px;
  text-transform: uppercase;
  transition: all 0.5s ease;
}

.navbar-nav {
  display: flex;
  flex-direction: row;
  padding-left: 0;
  margin-bottom: 0;
  list-style: none;
  align-items: center;
  justify-content: flex-end;
  gap: 10px;
}

.left-menu {
  margin-right: 32px;
}

.btn-menu, .btn-menu:hover {
  color: #000;
  background-color: #FEFFEF;
  border-color: #FEFFEF;
  padding: 5px 15px;
  border-radius: 25px;
  font-family: 'Arial, Helvetica, sans-serif';
  display: flex;
  align-items: center;
  gap: 5px;
}

.logomenu {
  height: 60px;
  width: auto; 
}

.imgperfil {
  height: 20px;
  width: auto;
}

</style>
