<template>
    <nav class="bg-blue-500 py-4">
    <div class="container mx-auto flex items-center justify-between px-4">
      <!-- Logo -->
      <div class="text-white font-bold text-xl">Geldwatch</div>

      <!-- Itens do Menu -->
      <ul class="flex space-x-4 text-white">
        <li><a href="#" class="hover:text-gray-300">Início</a></li>
        <li><a href="about" class="hover:text-gray-300">Sobre</a></li>
        <li><a href="faq" class="hover:text-gray-300">F.A.Q</a></li>
        <li><a href="#" class="hover:text-gray-300">Log in</a></li>
      </ul>
    </div>
  </nav>
</template>


<script>

export default {
    name: 'MenuLateral',
}
</script>