<!-- src/views/customer/CustomerLayout.vue -->
<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="#">
        <img src="@/assets/logo.png" alt="Logo" class="logo"> Meta Persona
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <router-link class="nav-link" to="/customer">Anasayfa</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/customer/user-form">Otelini Bul</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/customer/experience-form">Deneyim Listesi</router-link>
          </li>
        </ul>
      </div>
    </nav>
    <main class="containerr mt-4x">
      <slot></slot> 
    </main>
  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'CustomerLayout',
});
</script>

<style scoped>

.logo {
  height: 45px; 
  width: auto;  
  margin-right: 10px; 
}

.nav-link {
  font-size: 1.2rem; 
}



</style>
