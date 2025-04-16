<script>
import { RouterLink } from 'vue-router'

export default {
  name: 'NavbarComponent',
  components: {
    RouterLink
  }
}
</script>

<template>
  <nav class="flex items-center justify-between px-4 bg-gray-800 py-2" role="navigation">
    <RouterLink to="/">
      <img src="/images/burger-logo.png" alt="Logo MakeBurger" class="size-10" />
    </RouterLink>
    <div class="flex items-center gap-4">
      <RouterLink to="/" class="text-white border-b-2 border-transparent hover:border-white">Home</RouterLink>
      <RouterLink to="/orders" class="text-white border-b-2 border-transparent hover:border-white">Pedidos</RouterLink>
    </div>
  </nav>
</template>