<script setup lang="ts">
import router from './router';

</script>

<template>
  
  <div id="app">
    <nav>
      <router-link to="/">Inicio</router-link>
      <router-link to="/about">Temario</router-link>
      <router-link to="/Cuentos">Cuentos</router-link>
      <router-link to="/Cuentos">Test</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  background-color: #2c3e50;
  padding: 20px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
}

nav a {
  font-weight: bold;
  color: #fff;
  margin: 0 15px;
  text-decoration: none;
  transition: color 0.3s;
}

nav a:hover {
  color: #42b983;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
