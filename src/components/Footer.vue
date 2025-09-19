<template>
  <footer class="footer">
    <div class="container">
      <div class="row items-center justify-between">
        <!-- Texto -->
        <div class="col-md-6">
          <p class="footerp1">
            Todos os direitos reservados {{ year }} © - VetZ
          </p>
        </div>

        <!-- Ícones opcionais -->
        <div class="col-md-6 flex justify-end space-x-6">
          <a href="https://instagram.com" target="_blank" class="icon-link instagram">
            <i class="fa-brands fa-instagram"></i>
          </a>
          <a href="mailto:contato@vetz.com" class="icon-link email">
            <i class="fa-solid fa-envelope"></i>
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import { ref } from "vue";

// Ano atual dinâmico
const year = new Date().getFullYear();
</script>

<style scoped>
.footer {
  padding: 12px 0 10px 0;
  background-color: #B5E7A0;
  border-top: 1px solid #B5E7A0;
}

.footerp1 {
  color: #fff;
  font-size: 12px;
  line-height: 16px;
  letter-spacing: 1px;
  text-align: left;
  margin-top: 13px;
  font-family: 'Poppins-Regular';
}

/* Links de ícones */
.icon-link {
  color: #fff;
  font-size: 18px;
  transition: 0.3s;
}

.icon-link:hover {
  color: #000;
}
</style>