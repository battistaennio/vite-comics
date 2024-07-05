90<script>
    export default{
        name: "AppFooter",
    }
</script>

<template>
    <section>

        <a href="#">
            <div class="buy-box">
                <div class="img-container">
                    <img src="/src/assets/buy-comics-digital-comics.png" alt="digital comics">
                </div>
                <div class="shop-text">
                    <span>digital comics</span>
                </div>
            </div>
        </a>

        <a href="#">
            <div class="buy-box">
                <div class="img-container">
                    <img src="/src/assets/buy-comics-merchandise.png" alt="merchandise">
                </div>
                <div class="shop-text">
                    <span>dc merchandise</span>
                </div>
            </div>
        </a>

        <a href="#">
            <div class="buy-box">
                <div class="img-container">
                    <img src="/src/assets/buy-comics-subscriptions.png" alt="subscription">
                </div>
                <div class="shop-text">
                    <span>subscription</span>
                </div>
            </div>
        </a>

        <a href="#">
            <div class="buy-box">
                <div class="img-container">
                    <img src="/src/assets/buy-comics-shop-locator.png" alt="shop locator">
                </div>
                <div class="shop-text">
                    <span>dc shop locator</span>
                </div>
            </div>
        </a>

        <a href="#">
            <div class="buy-box">
                <div class="img-container">
                    <img src="/src/assets/buy-dc-power-visa.svg" alt="dc power visa">
                </div>
                <div class="shop-text">
                    <span>dc power visa</span>
                </div>
            </div>
        </a>

    </section>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

section{
    background-color: $primary-color;
    min-height: 130px;
    @include center();

    a{
        margin: 0 30px;

        .buy-box{
            @include center();

            .img-container{
                height: 50px;
                width: 50px;
                text-align: center;

                img{
                    height: 100%;
                }
            }

            .shop-text{
                color: white;
                text-transform: uppercase;
                margin-left: 15px;
                font-size: 0.7rem;
            }
        }
    }
}
</style>