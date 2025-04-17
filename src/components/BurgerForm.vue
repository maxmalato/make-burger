<script>
export default {
  name: 'BurgerFormComponent'
}
</script>

<template>
  <main class="max-w-2xl mx-auto my-8 p-8 bg-gray-50 rounded-lg shadow-md">
    <div class="text-center mb-6 text-gray-600 text-lg">Status da mensagem</div>
    <form class="space-y-6">
      <!-- Nome do cliente -->
      <div class="space-y-2">
        <label for="name" class="block font-semibold text-gray-700">Nome do cliente:</label>
        <input
          type="text"
          id="name"
          name="name"
          v-model="name"
          placeholder="Digite seu nome"
          class="w-full px-4 py-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500 focus:border-transparent transition-colors"
        >
      </div>

      <!-- Tipo de pão -->
      <div class="space-y-2">
        <label for="bread" class="block font-semibold text-gray-700">Tipo de pão:</label>
        <select
          id="bread"
          name="bread"
          v-model="bread"
          class="w-full px-4 py-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500 focus:border-transparent transition-colors"
        >
          <option value="white">Pão branco</option>
          <option value="wheat">Pão integral</option>
        </select>
      </div>

      <!-- Tipo de carne -->
      <div class="space-y-2">
        <label for="meat" class="block font-semibold text-gray-700">Tipo de carne:</label>
        <select
          id="meat"
          name="meat"
          v-model="meat"
          class="w-full px-4 py-3 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500 focus:border-transparent transition-colors"
        >
          <option value="beef">Carne de boi</option>
          <option value="chicken">Carne de frango</option>
        </select>
      </div>

      <!-- Adicionais -->
      <div class="space-y-2">
        <label class="block font-semibold text-gray-700">Adicionais:</label>
        <div class="flex space-x-4">
          <div class="flex items-center space-x-2">
            <input
              type="checkbox"
              id="tomato"
              name="tomato"
              v-model="tomato"
              class="w-5 h-5 text-green-500 rounded focus:ring-green-500"
            >
            <label for="tomato" class="text-gray-700">Tomate</label>
          </div>

          <div class="flex items-center space-x-2">
            <input
              type="checkbox"
              id="onion"
              name="onion"
              v-model="onion"
              class="w-5 h-5 text-green-500 rounded focus:ring-green-500"
            >
            <label for="onion" class="text-gray-700">Cebola</label>
          </div>

          <div class="flex items-center space-x-2">
            <input
              type="checkbox"
              id="lettuce"
              name="lettuce"
              v-model="lettuce"
              class="w-5 h-5 text-green-500 rounded focus:ring-green-500"
            >
            <label for="lettuce" class="text-gray-700">Alface</label>
          </div>
        </div>
      </div>

      <!-- Botão de envio -->
      <button
        type="submit"
        class="w-full bg-green-500 hover:bg-green-600 text-white font-semibold py-3 px-4 rounded-md transition-colors duration-200"
      >
        Enviar pedido
      </button>
    </form>
  </main>
</template>

<style scoped>
/* Removendo o estilo anterior pois agora usamos Tailwind */
</style>