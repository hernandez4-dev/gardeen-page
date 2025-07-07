<template>
  <div class="min-h-screen bg-gray-50 dark:bg-gray-900">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <div class="text-center mb-12">
        <h1 class="text-4xl font-bold text-gray-900 dark:text-white mb-4">
          Nuestros Servicios
        </h1>
        <p class="text-xl text-gray-600 dark:text-gray-300">
          Soluciones completas para tu jardín
        </p>
      </div>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Diseño de Jardines -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg overflow-hidden">
          <div class="bg-green-500 h-48 flex items-center justify-center">
            <svg class="w-16 h-16 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
            </svg>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
              Diseño de Jardines
            </h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              Creamos diseños únicos y personalizados que se adaptan a tu espacio y estilo de vida.
            </p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• Diseño conceptual</li>
              <li>• Planos detallados</li>
              <li>• Selección de plantas</li>
              <li>• Consultoría especializada</li>
            </ul>
          </div>
        </div>

        <!-- Mantenimiento -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg overflow-hidden">
          <div class="bg-green-600 h-48 flex items-center justify-center">
            <svg class="w-16 h-16 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path>
            </svg>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
              Mantenimiento
            </h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              Mantenemos tu jardín en perfectas condiciones durante todo el año.
            </p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• Poda y limpieza</li>
              <li>• Control de plagas</li>
              <li>• Fertilización</li>
              <li>• Riego automático</li>
            </ul>
          </div>
        </div>

        <!-- Instalación -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg overflow-hidden">
          <div class="bg-green-700 h-48 flex items-center justify-center">
            <svg class="w-16 h-16 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"></path>
            </svg>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
              Instalación
            </h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              Ejecutamos proyectos completos con la máxima calidad y profesionalismo.
            </p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• Preparación del terreno</li>
              <li>• Plantación</li>
              <li>• Sistemas de riego</li>
              <li>• Iluminación</li>
            </ul>
          </div>
        </div>

        <!-- Consultoría -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg overflow-hidden">
          <div class="bg-green-800 h-48 flex items-center justify-center">
            <svg class="w-16 h-16 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"></path>
            </svg>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
              Consultoría
            </h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              Asesoramiento experto para optimizar tu espacio verde.
            </p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• Evaluación del terreno</li>
              <li>• Recomendaciones</li>
              <li>• Planificación</li>
              <li>• Seguimiento</li>
            </ul>
          </div>
        </div>

        <!-- Paisajismo -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg overflow-hidden">
          <div class="bg-green-900 h-48 flex items-center justify-center">
            <svg class="w-16 h-16 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3.055 11H5a2 2 0 012 2v1a2 2 0 002 2 2 2 0 012 2v2.945M8 3.935V5.5A2.5 2.5 0 0010.5 8h.5a2 2 0 012 2 2 2 0 104 0 2 2 0 012-2h1.064M15 20.488V18a2 2 0 012-2h3.064M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
            </svg>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
              Paisajismo
            </h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              Transformamos espacios en paisajes naturales armoniosos.
            </p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• Diseño paisajístico</li>
              <li>• Elementos naturales</li>
              <li>• Integración ambiental</li>
              <li>• Sostenibilidad</li>
            </ul>
          </div>
        </div>

        <!-- Jardines Verticales -->
        <div class="bg-white dark:bg-gray-800 rounded-lg shadow-lg overflow-hidden">
          <div class="bg-green-950 h-48 flex items-center justify-center">
            <svg class="w-16 h-16 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16V4m0 0L3 8m4-4l4 4m6 0v12m0 0l4-4m-4 4l-4-4"></path>
            </svg>
          </div>
          <div class="p-6">
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">
              Jardines Verticales
            </h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              Soluciones innovadoras para espacios urbanos limitados.
            </p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• Muros verdes</li>
              <li>• Jardines colgantes</li>
              <li>• Sistemas hidropónicos</li>
              <li>• Mantenimiento especializado</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
// Componente Services
</script> 