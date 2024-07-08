<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppFooter from './components/AppFooter.vue';

  export default{
    name: "App",
    components: {
      AppHeader,
      AppJumbotron,
      AppFooter,

    }
  }
</script>

<template>
  <AppHeader />

  <AppJumbotron />

  <main>
    <!-- debug -->
    <div class="container">
      <h2 style="color: white; ">contenuto di pagina</h2>
    </div>

  </main>

  <AppFooter />


</template>

<style lang="scss">
  @use "./styles/general.scss" as *;
  @use "./styles/partials/variables" as *;

  main{
    background-color: #1c1c1c;
    // debug
    min-height: 100px;
    display: flex;
    align-items: center;
  }

</style>
