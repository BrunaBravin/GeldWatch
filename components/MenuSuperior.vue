<template>
  <nav class="bg-blue-500 py-4">
    <div class="container mx-auto flex items-center justify-between px-4">
      <!-- Logo -->
      <div class="text-white font-bold text-xl">Geldwatch</div>

      <!-- Itens do Menu -->
      <ul class="flex space-x-4 text-white">
        <NuxtLink to="/" class="hover:text-gray-300">Início</NuxtLink>
        <NuxtLink to="about" class="hover:text-gray-300">Sobre</NuxtLink>
        <NuxtLink to="faq" class="hover:text-gray-300">F.A.Q</NuxtLink>
        <NuxtLink to="teste" class="hover:text-gray-300">Log in</NuxtLink>
      </ul>


    </div>
  </nav>
</template>


<script>

export default {
  name: 'MenuLateral',
}
</script>