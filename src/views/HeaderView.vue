<template>
  <header>
    <nav class="bg-white border-gray-200 px-4 lg:px-6 py-2.5 dark:bg-green-500">
      <div class="flex justify-between items-center mx-auto max-w-screen-xl">
        <!-- Logo -->
        <router-link to="/" class="flex items-center">
          <img src="/public/img/earth.jpg" class="mr-3 h-6 sm:h-9" alt="SG" />
          <span class="text-xl font-semibold dark:text-white">Sunshine Green</span>
        </router-link>

        <!-- Menú y contacto alineados a la derecha -->
        <div class="flex items-center">
          <!-- Botón hamburguesa solo en móvil -->
          <button
            @click="isOpen = !isOpen"
            class="inline-flex items-center p-2 ml-3 text-sm text-gray-500 rounded-lg lg:hidden hover:bg-gray-100 dark:text-white dark:hover:bg-green-600"
          >
            <span class="sr-only">Abrir menú</span>
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </button>

          <!-- Menú navegación (escritorio) -->
          <ul class="hidden lg:flex flex-row items-center space-x-8 font-medium ml-8">
            <li>
              <router-link to="/" class="nav-item">Inicio</router-link>
            </li>
            <li>
              <router-link to="/about" class="nav-item">Nosotros</router-link>
            </li>
            <li>
              <router-link to="/services" class="nav-item">Servicios</router-link>
            </li>
            <li>
              <router-link to="/gallery" class="nav-item">Galería</router-link>
            </li>
            <li>
              <router-link to="/contact" class="nav-item"> Contacto </router-link>
            </li>
          </ul>
        </div>
      </div>

      <!-- Menú navegación responsive (móvil) -->
      <div :class="isOpen ? 'block' : 'hidden'" class="lg:hidden w-full mt-4">
        <ul class="flex flex-col font-medium space-y-2">
          <li>
            <router-link to="/" class="nav-item">Inicio</router-link>
          </li>
          <li>
            <router-link to="/about" class="nav-item">Nosotros</router-link>
          </li>
          <li>
            <router-link to="/services" class="nav-item">Servicios</router-link>
          </li>
          <li>
            <router-link to="/gallery" class="nav-item">Galería</router-link>
          </li>
          <li>
            <router-link to="/contact" class="nav-item"> Contacto </router-link>
          </li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script setup lang="ts">
import { ref } from 'vue'
const isOpen = ref(false)
</script>

<style scoped>
.nav-item {
  text-decoration: none;
  padding: 8px 16px;
  border-radius: 8px;
  transition: background-color 0.2s ease;
  color: #333;
}
.dark .nav-item {
  color: white;
}
.nav-item:hover {
  background-color: #f0f0f0;
}
.dark .nav-item:hover {
  background-color: #256d1b;
}
</style>
