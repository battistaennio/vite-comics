<script>
    export default{
        name: "ComicCard",
        props: {details: Object},
    }
</script>

<template>
    <div class="comic-card">
        <div class="img-container">
            <img :src="details.thumb" :alt="details.series">
        </div>
        <h3>{{details.series}}</h3>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

.comic-card{
    width: calc(100% / 6 - 25px);
    margin: 10px 0;

    .img-container{
        height: 200px;

        img{
        height: 100%;
        width: 100%;
        }
    }

    h3{
    color: white;
    text-align: center;
    text-transform: uppercase;
    margin-top: 10px;
    font-weight: 100;
    }

}

</style>