<script>
import AppHeader from './components/AppHeader.vue';

  export default{
    name: "App",
    components: {
      AppHeader,

    }
  }
</script>

<template>
  <AppHeader />

  <main>
    <!-- debug -->
    <div class="container">
      <h2 style="color: white; ">contenuto di pagina</h2>
    </div>

  </main>

  
</template>

<style lang="scss">
  @use "./styles/general.scss" as *;
  @use "./styles/partials/variables" as *;

  main{
    background-color: #1c1c1c;
    // debug
    min-height: 150px;
    display: flex;
    align-items: center;
  }

</style>
