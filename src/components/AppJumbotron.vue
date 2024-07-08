<script>
    export default{
        name: "AppJumbotron",
    }
</script>

<template>
    <img src="../assets/jumbotron.jpg" alt="jumbotron">
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

img{
    height: 350px;
    width: 100%;
    object-fit: cover;
    object-position: top;
    display: block;
}
</style>