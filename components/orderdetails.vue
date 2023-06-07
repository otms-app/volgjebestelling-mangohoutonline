<template>
  <!-- Footer -->
  <div class="footer border-top">
    <div class="text-center">
      <p class="footer-p">
        &copy; {{ new Date().getFullYear() }} Mangohoutonline<br />Aan de
        informatie op onze website kunnen geen rechten worden ontleend
      </p>
    </div>
  </div>
</template>

<script>
import { inject } from 'vue';

export default {};
</script>

<style>
.footer {
  margin-top: 15px;
  font-size: 11px;
  font-family: sans-serif;
}

.footer-p {
  margin-top: 15px;
}
</style>
