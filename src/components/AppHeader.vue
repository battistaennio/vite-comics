<script>
    export default{
        name: "AppHeader",
        data(){
            return {
                links: [
                    {
                        text: "characters",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "comics",
                        url: "#",
                        current: true,
                    },
                    {
                        text: "movies",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "tv",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "games",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "collectibles",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "videos",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "fans",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "news",
                        url: "#",
                        current: false,
                    },
                    {
                        text: "shop",
                        url: "#",
                        current: false,
                    },
                ]
            }
        }
    }


</script>

<template>
    <header>
        <div class="container">
            <nav>
                <ul>
                    <li>
                        <a href="#">
                            <img src="/src/assets/dc-logo.png" alt="DC logo">
                        </a>
                    </li>
                </ul>

                <ul class="nav">
                    <li v-for="(link, index) in links" :key="index">
                        <a :href="link.url" :class="{active: link.current}">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;


header{
    height: 90px;

    nav{
        @include center("between");

        ul{
            display: flex;

            img{
                width: 60px;
                margin: 15px 0;
            }
        }

        .nav{

            a{
                text-transform: uppercase;
                font-size: 0.6rem;
                margin: 0 15px;
                padding-bottom: 31px;
                font-weight: 600;
                &:hover{
                    border-bottom: 5px solid $primary-color;
                }
            }

            .active{
                border-bottom: 5px solid $primary-color;
                color: $primary-color;
            }
        }
    }
}
</style>