90<script>
    export default{
        name: "AppHeader",
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
                    <li>
                        <a href="#">characters</a>
                    </li>
                    <li>
                        <a href="#">comics</a>
                    </li>
                    <li>
                        <a href="#">movies</a>
                    </li>
                    <li>
                        <a href="#">tv</a>
                    </li>
                    <li>
                        <a href="#">games</a>
                    </li>
                    <li>
                        <a href="#">collectibles</a>
                    </li>
                    <li>
                        <a href="#">videos</a>
                    </li>
                    <li>
                        <a href="#">fans</a>
                    </li>
                    <li>
                        <a href="#">news</a>
                    </li>
                    <li>
                        <a href="#">shop</a>
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
        }
    }
}
</style>