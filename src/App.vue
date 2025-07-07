<template>
  <div>
    <HeaderView />
    <main>
      <router-view />
    </main>
    <FooterView />
  </div>
</template>

<script lang="ts" setup>
import HeaderView from '@/views/HeaderView.vue'
import FooterView from './views/FooterView.vue'
</script>
