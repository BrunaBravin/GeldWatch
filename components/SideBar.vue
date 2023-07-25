<template>
  <div id="view" class="h-full w-screen flex flex-row" :class="{ 'sidenav-aberta': sidenav }"
    @click.away="sidenav = false">




    <button @click="sidenav = true"
      class="p-2 border-2 bg-white rounded-md border-gray-200 shadow-lg text-gray-500 focus:bg-teal-500 focus:outline-none focus:text-white absolute top-0 left-0 sm:hidden">
      <!-- Coloque aqui o código SVG para o ícone do botão -->

    </button>





    <div id="sidebar"
      class="bg-white h-screen md:block shadow-xl px-3 w-30 md:w-60 lg:w-60 overflow-x-hidden transition-transform duration-300 ease-in-out">
      <div class="space-y-6 md:space-y-10 mt-10">
        <h1 class="font-bold text-4xl text-center md:hidden">
          D<span class="text-teal-600">.</span>
        </h1>
        <div id="profile" class="space-y-3">

          <!-- Imagem de perfil do usuário -->
          <img
            src="https://images.unsplash.com/photo-1628157588553-5eeea00af15c?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80"
            alt="Avatar do usuário" class="w-10 md:w-16 rounded-full mx-auto" />

          <!-- Nome do usuário -->
          <div>
            <h2 class="font-medium text-xs md:text-sm text-center text-teal-500">
              Eduard Pantazi
            </h2>

            <!-- Tipo de usuário -->
            <p class="text-xs text-gray-500 text-center">Administrador</p>

          </div>

        </div>

        <div class="flex border-2 border-gray-200 rounded-md focus-within:ring-2 ring-teal-500">

          <input type="text" class="w-full rounded-tl-md rounded-bl-md px-2 py-3 text-sm text-gray-600 focus:outline-none"
            placeholder="Pesquisar" />


          <button class="rounded-tr-md rounded-br-md px-2 py-3 hidden md:block">
            <!-- Código SVG para o ícone de pesquisa -->
            <svg class="w-4 h-4 fill-current" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd"
                d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
                clip-rule="evenodd"></path>
            </svg>
          </button>


        </div>
        <div id="menu" class="flex flex-col space-y-2">
          <a href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:text-base rounded-md transition duration-150 ease-in-out">
            <!-- Coloque aqui o código SVG para o ícone do dashboard -->

            <svg class="w-6 h-6 fill-current inline-block bi bi-bar-chart-line-fill" fill="currentColor" viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg" width="16" height="16">
              <path
                d="M11 2a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v12h.5a.5.5 0 0 1 0 1H.5a.5.5 0 0 1 0-1H1v-3a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v3h1V7a1 1 0 0 1 1-1h2a1 1 0 0 1 1 1v7h1V2z" />
            </svg>

            <span class="">Dashboard</span>

          </a>
          <a href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out">
            <!-- Coloque aqui o código SVG para o ícone de produtos -->

            <svg class="w-6 h-6 fill-current inline-block bi bi-currency-bitcoin" fill="currentColor" viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg" width="16" height="16">
              <path
                d="M5.5 13v1.25c0 .138.112.25.25.25h1a.25.25 0 0 0 .25-.25V13h.5v1.25c0 .138.112.25.25.25h1a.25.25 0 0 0 .25-.25V13h.084c1.992 0 3.416-1.033 3.416-2.82 0-1.502-1.007-2.323-2.186-2.44v-.088c.97-.242 1.683-.974 1.683-2.19C11.997 3.93 10.847 3 9.092 3H9V1.75a.25.25 0 0 0-.25-.25h-1a.25.25 0 0 0-.25.25V3h-.573V1.75a.25.25 0 0 0-.25-.25H5.75a.25.25 0 0 0-.25.25V3l-1.998.011a.25.25 0 0 0-.25.25v.989c0 .137.11.25.248.25l.755-.005a.75.75 0 0 1 .745.75v5.505a.75.75 0 0 1-.75.75l-.748.011a.25.25 0 0 0-.25.25v1c0 .138.112.25.25.25L5.5 13zm1.427-8.513h1.719c.906 0 1.438.498 1.438 1.312 0 .871-.575 1.362-1.877 1.362h-1.28V4.487zm0 4.051h1.84c1.137 0 1.756.58 1.756 1.524 0 .953-.626 1.45-2.158 1.45H6.927V8.539z" />
            </svg>

            <span class="">Crypto</span>

          </a>

          <a href=""
            class="text-sm font-medium text-gray-700 py-2 px-2 hover:bg-teal-500 hover:text-white hover:scale-105 rounded-md transition duration-150 ease-in-out">
            <!-- Coloque aqui o código SVG para o ícone de relatórios -->

            <svg class="w-6 h-6 fill-current inline-block bi bi-bank" fill="currentColor" viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg" width="16" height="16">
              <path
                d="M8 .95 14.61 4h.89a.5.5 0 0 1 .5.5v2a.5.5 0 0 1-.5.5H15v7a.5.5 0 0 1 .485.379l.5 2A.5.5 0 0 1 15.5 17H.5a.5.5 0 0 1-.485-.621l.5-2A.5.5 0 0 1 1 14V7H.5a.5.5 0 0 1-.5-.5v-2A.5.5 0 0 1 .5 4h.89L8 .95zM3.776 4h8.447L8 2.05 3.776 4zM2 7v7h1V7H2zm2 0v7h2.5V7H4zm3.5 0v7h1V7h-1zm2 0v7H12V7H9.5zM13 7v7h1V7h-1zm2-1V5H1v1h14zm-.39 9H1.39l-.25 1h13.72l-.25-1z" />
            </svg>

            <span class="">Relatórios</span>

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