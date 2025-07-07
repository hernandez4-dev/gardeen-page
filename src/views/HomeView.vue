<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section class="relative bg-gradient-to-br from-green-50 to-green-100 dark:from-gray-900 dark:to-gray-800">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24">
        <div class="text-center">
          <h1 class="text-5xl md:text-6xl font-bold text-gray-900 dark:text-white mb-6">
            Bienvenidos a
            <span class="text-green-600">Sunshine Green</span>
          </h1>
          <p class="text-xl md:text-2xl text-gray-600 dark:text-gray-300 mb-8 max-w-3xl mx-auto">
            Transformamos espacios ordinarios en extraordinarios jardines. 
            Conectamos personas con la naturaleza, creando oasis verdes que 
            mejoran tu calidad de vida.
          </p>
          <div class="flex flex-col sm:flex-row gap-4 justify-center">
            <router-link
              to="/services"
              class="bg-green-600 text-white px-8 py-4 rounded-lg text-lg font-semibold hover:bg-green-700 transition-colors duration-200"
            >
              Nuestros Servicios
            </router-link>
            <router-link
              to="/contact"
              class="border-2 border-green-600 text-green-600 dark:text-green-400 px-8 py-4 rounded-lg text-lg font-semibold hover:bg-green-600 hover:text-white transition-colors duration-200"
            >
              Contáctanos
            </router-link>
          </div>
        </div>
      </div>
    </section>

    <!-- Servicios Destacados -->
    <section class="py-16 bg-white dark:bg-gray-900">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-12">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-4">
            Servicios Destacados
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            Soluciones completas para transformar tu espacio verde
          </p>
        </div>

        <div class="grid md:grid-cols-3 gap-8">
          <div class="text-center p-6">
            <div class="bg-green-100 dark:bg-green-900 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-green-600 dark:text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">Diseño de Jardines</h3>
            <p class="text-gray-600 dark:text-gray-300">
              Creamos diseños únicos y personalizados que se adaptan a tu espacio y estilo de vida.
            </p>
          </div>

          <div class="text-center p-6">
            <div class="bg-green-100 dark:bg-green-900 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-green-600 dark:text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">Mantenimiento</h3>
            <p class="text-gray-600 dark:text-gray-300">
              Mantenemos tu jardín en perfectas condiciones durante todo el año.
            </p>
          </div>

          <div class="text-center p-6">
            <div class="bg-green-100 dark:bg-green-900 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
              <svg class="w-8 h-8 text-green-600 dark:text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 16V4m0 0L3 8m4-4l4 4m6 0v12m0 0l4-4m-4 4l-4-4"></path>
              </svg>
            </div>
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-3">Jardines Verticales</h3>
            <p class="text-gray-600 dark:text-gray-300">
              Soluciones innovadoras para espacios urbanos limitados.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Por qué elegirnos -->
    <section class="py-16 bg-gray-50 dark:bg-gray-800">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid lg:grid-cols-2 gap-12 items-center">
          <div>
            <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-6">
              ¿Por qué elegir Sunshine Green?
            </h2>
            <div class="space-y-6">
              <div class="flex items-start">
                <div class="flex-shrink-0">
                  <div class="w-8 h-8 bg-green-600 rounded-full flex items-center justify-center">
                    <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                    </svg>
                  </div>
                </div>
                <div class="ml-4">
                  <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Experiencia Comprobada</h3>
                  <p class="text-gray-600 dark:text-gray-300">Más de 10 años transformando espacios verdes con resultados excepcionales.</p>
                </div>
              </div>

              <div class="flex items-start">
                <div class="flex-shrink-0">
                  <div class="w-8 h-8 bg-green-600 rounded-full flex items-center justify-center">
                    <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                    </svg>
                  </div>
                </div>
                <div class="ml-4">
                  <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Equipo Profesional</h3>
                  <p class="text-gray-600 dark:text-gray-300">Especialistas certificados en jardinería, paisajismo y diseño sostenible.</p>
                </div>
              </div>

              <div class="flex items-start">
                <div class="flex-shrink-0">
                  <div class="w-8 h-8 bg-green-600 rounded-full flex items-center justify-center">
                    <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                    </svg>
                  </div>
                </div>
                <div class="ml-4">
                  <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Sostenibilidad</h3>
                  <p class="text-gray-600 dark:text-gray-300">Utilizamos técnicas eco-friendly y plantas nativas para cuidar el medio ambiente.</p>
                </div>
              </div>

              <div class="flex items-start">
                <div class="flex-shrink-0">
                  <div class="w-8 h-8 bg-green-600 rounded-full flex items-center justify-center">
                    <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                    </svg>
                  </div>
                </div>
                <div class="ml-4">
                  <h3 class="text-lg font-semibold text-gray-900 dark:text-white">Garantía Total</h3>
                  <p class="text-gray-600 dark:text-gray-300">Respaldamos nuestro trabajo con garantías completas y servicio post-venta.</p>
                </div>
              </div>
            </div>
          </div>

          <div class="bg-green-100 dark:bg-green-900 p-8 rounded-lg">
            <h3 class="text-2xl font-semibold text-green-800 dark:text-green-200 mb-6">
              Nuestros Números Hablan
            </h3>
            <div class="grid grid-cols-2 gap-6">
              <div class="text-center">
                <div class="text-3xl font-bold text-green-600 dark:text-green-400 mb-2">150+</div>
                <div class="text-green-700 dark:text-green-300 text-sm">Proyectos Exitosos</div>
              </div>
              <div class="text-center">
                <div class="text-3xl font-bold text-green-600 dark:text-green-400 mb-2">50+</div>
                <div class="text-green-700 dark:text-green-300 text-sm">Clientes Felices</div>
              </div>
              <div class="text-center">
                <div class="text-3xl font-bold text-green-600 dark:text-green-400 mb-2">10+</div>
                <div class="text-green-700 dark:text-green-300 text-sm">Años de Experiencia</div>
              </div>
              <div class="text-center">
                <div class="text-3xl font-bold text-green-600 dark:text-green-400 mb-2">100%</div>
                <div class="text-green-700 dark:text-green-300 text-sm">Satisfacción</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="py-16 bg-green-600">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-3xl md:text-4xl font-bold text-white mb-6">
          ¿Listo para transformar tu espacio?
        </h2>
        <p class="text-xl text-green-100 mb-8 max-w-2xl mx-auto">
          Contáctanos hoy mismo para una consulta gratuita y descubre cómo podemos 
          convertir tu jardín en el oasis que siempre soñaste.
        </p>
        <router-link
          to="/contact"
          class="bg-white text-green-600 px-8 py-4 rounded-lg text-lg font-semibold hover:bg-gray-100 transition-colors duration-200"
        >
          Solicitar Consulta Gratuita
        </router-link>
      </div>
    </section>
  </div>
</template>

<script lang="ts" setup>
// Componente Home
</script>
