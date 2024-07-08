<script>
    export default{
        name: "ListComics",
    }
</script>

<template>
    <section>
        <div class="container">
            <h2>current series</h2>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    section{
        background-color: #1c1c1c;
        padding: 40px 0;
        position: relative;
        // debug
        min-height: 100px;

        h2{
            color: white;
            text-transform: uppercase;
            display: inline-block;
            padding: 10px 20px;
            background-color: $primary-color;
            position: absolute;
            top: -25px;
        }
    }
</style>