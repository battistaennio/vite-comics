90<script>
    export default{
        name: "AppFooter",
    }
</script>

<template>

    <section id="footer-buy">

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

    <section id="footer-list_container">
        <div class="container">
            <div id="footer-list">
                <div>
                    <ul>
                        <li>
                            <a href="#">
                                dc comics
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Characters
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Comics
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Movies
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                TV
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Games
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Videos
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                News
                            </a>
                        </li>
                    </ul>

                    <ul>
                        <li>
                            <a href="#">
                                shop
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Shop DC
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Shop DC Collectibles
                            </a>
                        </li>
                    </ul>
                </div>

                <ul>
                    <li>
                        <a href="#">
                            dc
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            Characters
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            Comics
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            Movies
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            TV
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            Games
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            Videos
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            News
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            TV
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            Games
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            Videos
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            News
                        </a>
                    </li>
                </ul>

                <ul>
                    <li>
                        <a href="#">
                            sites
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            DC
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            MAD Magazine
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            DC Kids
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            DC Universe
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            DC Power Visa
                        </a>
                    </li>
                </ul>
            </div>

            <div id="footer-logo">
                <img src="/src/assets/dc-logo-bg.png" alt="footer logo">
            </div>

        </div>
    </section>

    <section id="footer-social">
        <div class="container">
            <button>sign-up now!</button>

            <div id="social-container">
                <h3>follow us</h3>
                <div class="img-container">
                    <a href="#">
                        <img src="/src/assets/footer-facebook.png" alt="">
                    </a>
                    <a href="#">
                        <img src="/src/assets/footer-twitter.png" alt="">
                    </a>
                    <a href="#">
                        <img src="/src/assets/footer-youtube.png" alt="">
                    </a>
                    <a href="#">
                        <img src="/src/assets/footer-pinterest.png" alt="">
                    </a>
                    <a href="#">
                        <img src="/src/assets/footer-periscope.png" alt="">
                    </a>
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

section#footer-buy{
    background-color: $primary-color;
    height: 130px;
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

section#footer-list_container{
    height: 300px;
    background-size: cover;
    background-image: url("../assets/footer-bg.jpg");
    overflow-y: hidden;

    .container{
        height: 100%;
        @include center("between");

        #footer-list{
            display: flex;
            flex-wrap: wrap;
            flex-shrink: unset;
            ul{
                margin: 20px 10px;
                li{
                    a{
                        display: inline-block;
                        color: gray;
                        margin-bottom: 2px;
                        font-size: 0.8rem;

                        &:hover{
                            text-decoration: underline;
                        }
                    }

                    &:first-child{

                        a{
                            color: white;
                            text-transform: uppercase;
                            font-weight: 600;
                            font-size: 1.2rem;
                            margin-bottom: 7px;
                        }
                    }
                }
            }
        }

        #footer-logo{
            width: 450px;
            height: 450px;
        }
    }
}

section#footer-social{
    height: 100px;
    background-color: #303030;
    .container{
        height: 100%;
        @include center("between");

        button{
            text-transform: uppercase;
            color: white;
            border-radius: 0;
            border: 3px solid $primary-color;
            background: none;
            padding: 10px 15px;
            cursor: pointer;
        }

        #social-container{
            @include center();
            h3{
            text-transform: uppercase;
            color: $primary-color;
            margin: 0 10px;
            }

            img{
                margin-left: 15px;
                width: 30px;
            }
        }
    }
}

</style>