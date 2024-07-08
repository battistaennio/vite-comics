<script>
    export default{
        name: "ComicCard",
    }
</script>

<template>
    <div class="comic-card">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="">
        <h3>titolo</h3>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.comic-card{
    width: calc(100% / 6);
}

h3{
    color: white;
    text-align: center;
    text-transform: uppercase;
    margin: 10px 0;
}

</style>