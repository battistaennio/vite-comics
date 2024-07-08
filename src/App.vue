<script>
import AppHeader from './components/AppHeader.vue';
import ListComics from './components/ListComics.vue';
import AppFooter from './components/AppFooter.vue';

  export default{
    name: "App",
    components: {
      AppHeader,
      ListComics,
      AppFooter,

    }
  }
</script>

<template>
  <AppHeader />

  <main>
    <ListComics />
  </main>

  <AppFooter />


</template>

<style lang="scss">
  @use "./styles/general.scss" as *;
  @use "./styles/partials/variables" as *;
</style>
