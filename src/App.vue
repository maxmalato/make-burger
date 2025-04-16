<script setup>
import { RouterView } from 'vue-router'
import NavbarComponent from '@/components/Navbar.vue'
import FooterComponent from '@/components/Footer.vue'
</script>

<template>
  <NavbarComponent />
  <RouterView />
  <FooterComponent />
</template>
