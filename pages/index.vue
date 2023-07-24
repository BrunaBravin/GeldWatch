<template>

  <div>
  <!-- Menu superior-->
  <MenuSuperior/>

  <SideBar />

  <!-- Resto do Conteúdo -->
  <div class="container mx-auto py-8 px-4">
    <h1 class="text-3xl font-bold mb-4">Bem-vindo ao Meu Site</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum suscipit gravida ultrices. Sed eget
      efficitur odio. Nulla facilisi.</p>
  </div>
  </div>


</template>

<script>
import MenuSuperior from '../components/MenuSuperior.vue';
import SideBar from '../components/SideBar.vue';
export default {
    name: "index",
    components: { MenuSuperior, SideBar }
}
</script>
