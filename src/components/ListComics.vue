<script>
    import ComicCard from './ComicCard.vue';
    import comics from '../assets/dc-comics 2.json'

    export default{
        name: "ListComics",
        components: {
            ComicCard,
        },
        data() {
            return{
                list: comics,
            }
        }
    }
</script>

<template>
    <section>
        <div class="container">
            <h2>current series</h2>

            <div class="cards-container">
                <ComicCard />
            </div>
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

        h2{
            color: white;
            text-transform: uppercase;
            display: inline-block;
            padding: 10px 20px;
            background-color: $primary-color;
            position: absolute;
            top: -25px;
        }

        .cards-container{
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
        }
    }
</style>