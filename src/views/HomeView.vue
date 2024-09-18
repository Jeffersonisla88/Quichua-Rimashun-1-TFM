<template>
  <div class="home">
    <title>Quichua Rimashun</title>
    <h2>Comienza tu aventura en el mundo del quichua</h2>
    <p>Descubre juegos, canciones y muchas sorpresas mientras aprendes.</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import backgroundImage from '@/assets/logo.png'; // Importa la imagen

export default defineComponent({
  name: 'Home',
  data() {
    return {
      backgroundImage, // Añade la imagen a los datos del componente
    };
  },
});
</script>

<style scoped>
.home {
  padding: 40px 20px;
  background-image: url('@/assets/logo.png'); /* Uso de la imagen como fondo */
  background-size: cover;
  background-position: center;
  position: relative;
  height: 100vh;
}

.home::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(255, 255, 255, 0.7); /* Fondo opaco */
  z-index: 1;
}

h2, p {
  position: relative;
  z-index: 2;
}

h2 {
  margin-bottom: 20px;
  font-size: 1.8rem;
  color: #000000;
}

p {
  font-size: 1.1rem;
  color: #382a2a;
}
</style>
