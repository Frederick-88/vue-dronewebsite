<template>
  <div class="app" id="app">
    <router-view />
  </div>
</template>

<style>
html {
  scroll-behavior: smooth;
}
.app {
  font-family: "Poppins", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.button-fx {
  border: 0 !important;
  padding: 0.75rem 1.5rem !important;
  background-image: linear-gradient(55deg, #0250c5 0%, #d43f8d 100%);
  transition: 0.3s ease-in;
}
.button-fx:hover {
  background-image: linear-gradient(55deg, #d43f8d 0%, #0250c5);
}
</style>
