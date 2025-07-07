<template>
  <div class="min-h-screen bg-gray-50 dark:bg-gray-900">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <div class="text-center mb-12">
        <h1 class="text-4xl font-bold text-gray-900 dark:text-white mb-4">Galería de Proyectos</h1>
        <p class="text-xl text-gray-600 dark:text-gray-300">
          Descubre algunos de nuestros trabajos más destacados
        </p>
      </div>

      <!-- Filtros -->
      <div class="flex flex-wrap justify-center gap-4 mb-8">
        <button
          v-for="categoria in categorias"
          :key="categoria.id"
          @click="categoriaActiva = categoria.id"
          :class="[
            'px-4 py-2 rounded-full text-sm font-medium transition-colors duration-200',
            categoriaActiva === categoria.id
              ? 'bg-green-600 text-white'
              : 'bg-white text-gray-700 hover:bg-gray-100 dark:bg-gray-800 dark:text-gray-300 dark:hover:bg-gray-700',
          ]"
        >
          {{ categoria.nombre }}
        </button>
      </div>

      <!-- Galería -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div
          v-for="proyecto in proyectosFiltrados"
          :key="proyecto.id"
          class="bg-white dark:bg-gray-800 rounded-lg shadow-lg overflow-hidden hover:shadow-xl transition-shadow duration-300"
        >
          <div class="relative h-64 bg-gray-200 dark:bg-gray-700">
            <img
              :src="proyecto.imagen"
              :alt="proyecto.titulo"
              class="object-cover w-full h-full absolute inset-0"
            />
            <div class="absolute inset-0 bg-gradient-to-t from-black/50 to-transparent"></div>
            <div class="absolute bottom-4 left-4 right-4">
              <h3 class="text-white text-lg font-semibold mb-2">{{ proyecto.titulo }}</h3>
              <p class="text-gray-200 text-sm">{{ proyecto.ubicacion }}</p>
            </div>
            <div class="absolute top-4 right-4">
              <span class="bg-green-600 text-white px-2 py-1 rounded-full text-xs font-medium">
                {{ proyecto.categoria }}
              </span>
            </div>
          </div>

          <div class="p-6">
            <p class="text-gray-600 dark:text-gray-300 text-sm mb-4">
              {{ proyecto.descripcion }}
            </p>

            <div class="flex items-center justify-between">
              <div class="flex items-center space-x-2">
                <span class="text-green-600 text-sm font-medium">{{ proyecto.area }}</span>
                <span class="text-gray-400 text-sm">•</span>
                <span class="text-gray-500 dark:text-gray-400 text-sm">{{
                  proyecto.duracion
                }}</span>
              </div>

              <button class="text-green-600 hover:text-green-700 text-sm font-medium">
                Ver más →
              </button>
            </div>
          </div>
        </div>
      </div>

      <!-- Estadísticas -->
      <div class="mt-16 bg-white dark:bg-gray-800 rounded-lg shadow-lg p-8">
        <h2 class="text-2xl font-semibold text-gray-900 dark:text-white text-center mb-8">
          Nuestros Números
        </h2>

        <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
          <div class="text-center">
            <div class="text-3xl font-bold text-green-600 mb-2">150+</div>
            <div class="text-gray-600 dark:text-gray-300">Proyectos Completados</div>
          </div>

          <div class="text-center">
            <div class="text-3xl font-bold text-green-600 mb-2">50+</div>
            <div class="text-gray-600 dark:text-gray-300">Clientes Satisfechos</div>
          </div>

          <div class="text-center">
            <div class="text-3xl font-bold text-green-600 mb-2">10+</div>
            <div class="text-gray-600 dark:text-gray-300">Años de Experiencia</div>
          </div>

          <div class="text-center">
            <div class="text-3xl font-bold text-green-600 mb-2">5</div>
            <div class="text-gray-600 dark:text-gray-300">Premios Ganados</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref, computed } from 'vue'

const categoriaActiva = ref('todos')

const categorias = [
  { id: 'todos', nombre: 'Todos' },
  { id: 'diseno', nombre: 'Diseño' },
  { id: 'mantenimiento', nombre: 'Mantenimiento' },
  { id: 'paisajismo', nombre: 'Paisajismo' },
  { id: 'verticales', nombre: 'Jardines Verticales' },
]

const proyectos = [
  {
    id: 1,
    titulo: 'Jardín Residencial Moderno',
    ubicacion: 'San Salvador',
    categoria: 'Diseño',
    categoriaId: 'diseno',
    descripcion: 'Jardín contemporáneo con elementos minimalistas y plantas nativas.',
    area: '200 m²',
    duracion: '3 meses',
    imagen: 'img/jardines/sanbenito.jpg',
  },
  {
    id: 2,
    titulo: 'Muro Verde Corporativo',
    ubicacion: 'San Benito, San Salvador',
    categoria: 'Jardines Verticales',
    categoriaId: 'verticales',
    descripcion: 'Instalación de muro verde en fachada residencial',
    area: '150 m²',
    duracion: '2 meses',
    imagen: 'img/jardines/dos.jpg',
  },
  {
    id: 3,
    titulo: 'Parque Recreativo',
    ubicacion: 'San Miguel, El Salvador',
    categoria: 'Paisajismo',
    categoriaId: 'paisajismo',
    descripcion: 'Diseño y construcción de parque público con áreas recreativas y jardines.',
    area: '2,500 m²',
    duracion: '6 meses',
    imagen: 'img/jardines/tres.jpg',
  },
  {
    id: 4,
    titulo: 'Jardín Botánico Privado',
    ubicacion: 'La Libertad',
    categoria: 'Diseño',
    categoriaId: 'diseno',
    descripcion: 'Jardín botánico con más de 100 especies de plantas y senderos educativos.',
    area: '800 m²',
    duracion: '8 meses',
    imagen: 'img/jardines/cuantro.jpg',
  },
  {
    id: 5,
    titulo: 'Mantenimiento Comercial',
    ubicacion: 'Mall Cascadas, San Salvador',
    categoria: 'Mantenimiento',
    categoriaId: 'mantenimiento',
    descripcion: 'Servicio de mantenimiento integral para centro comercial.',
    area: '1,200 m²',
    duracion: 'Ongoing',
    imagen: 'img/jardines/sanmiguel.jpg',
  },
  {
    id: 6,
    titulo: 'Terraza Verde Urbana',
    ubicacion: 'Cuscatlán',
    categoria: 'Jardines Verticales',
    categoriaId: 'verticales',
    descripcion: 'Terraza verde en casa de campo.',
    area: '300 m²',
    duracion: '4 meses',
    imagen: 'img/jardines/terraza.jpg',
  },
]

const proyectosFiltrados = computed(() => {
  if (categoriaActiva.value === 'todos') {
    return proyectos
  }
  return proyectos.filter((proyecto) => proyecto.categoriaId === categoriaActiva.value)
})
</script>
