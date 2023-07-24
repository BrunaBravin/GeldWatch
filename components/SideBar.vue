<template>
    <div
    id="view"
    class="h-full w-screen flex flex-row"
    :class="{ 'sidenav-aberta': sidenav }"
    @click.away="sidenav = false"
  >




    <button
      @click="sidenav = true"
      class="p-2 border-2 bg-white rounded-md border-gray-200 shadow-lg text-gray-500 focus:bg-teal-500 focus:outline-none focus:text-white absolute top-0 left-0 sm:hidden"
    >
      <!-- Coloque aqui o código SVG para o ícone do botão -->
      
    </button>




    
    <div
      id="sidebar"
      class="bg-white h-screen md:block shadow-xl px-3 w-30 md:w-60 lg:w-60 overflow-x-hidden transition-transform duration-300 ease-in-out"
    >
      <div class="space-y-6 md:space-y-10 mt-10">
        <h1 class="font-bold text-4xl text-center md:hidden">
          D<span class="text-teal-600">.</span>
        </h1>
        <h1 class="hidden md:block font-bold text-sm md:text-xl text-center">
          Dashwind<span class="text-teal-600">.</span>
        </h1>
        <div id="profile" class="space-y-3">
          <img
            src="https://images.unsplash.com/photo-1628157588553-5eeea00af15c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80"
            alt="Avatar do usuário"
            class="w-10 md:w-16 rounded-full mx-auto"
          />
          <div>
            <h2 class="font-medium text-xs md:text-sm text-center text-teal-500">
              Eduard Pantazi
            </h2>
            <p class="text-xs text-gray-500 text-center">Administrador</p>
          </div>
        </div>
        <div class="flex border-2 border-gray-200 rounded-md focus-within:ring-2 ring-teal-500">
          <input
            type="text"
            class="w-full rounded-tl-md rounded-bl-md px-2 py-3 text-sm text-gray-600 focus:outline-none"
            placeholder="Pesquisar"
          />
          <button class="rounded-tr-md rounded-br-md px-2 py-3 hidden md:block">
            <!-- Coloque aqui o código SVG para o ícone de pesquisa -->
          </button>
        </div>
        <div id="menu" class="flex flex-col space-y-2">
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:text-base rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone do dashboard -->
            <svg
          class="w-5 h-5 fill-current"
          fill="currentColor"
          viewBox="0 0 20 20"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
            clip-rule="evenodd"
          ></path>
        </svg>
            <span class="">Dashboard</span>
          </a>
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone de produtos -->
            <span class="">Produtos</span>
          </a>
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone de relatórios -->
            <span class="">Relatórios</span>
          </a>
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone de mensagens -->
            <span class="">Mensagens</span>
          </a>
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone do calendário -->
            <span class="">Calendário</span>
          </a>
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone de tabela -->
            <span class="">Tabela</span>
          </a>
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone de componentes UI -->
            <span class="">Componentes UI</span>
          </a>
          <a
            href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out"
          >
            <!-- Coloque aqui o código SVG para o ícone de usuários -->
            <span class="">Usuários</span>
          </a>
        </div>
      </div>
    </div>
  </div>
  </template>
  
  <script>
  export default {
    name: 'SideBar',
    data() {
      return {
        sidenav: false,
      };
    },
  };
  </script>
  
  <style>
  /* Add your custom styles or Tailwind CSS classes here */
  .sidenav-open #sidebar {
    transform: translateX(0);
  }
  </style>