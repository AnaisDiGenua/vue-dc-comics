<template>
    <footer>
        <!-- footer top -->
            <div class="footer-top">
                <div class="container">
                    <ul>
                        <li>
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <a href="#">Digital comics</a>
                        </li>
                        <li>
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <a href="#">Digital comics</a>
                        </li>
                        <li>
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <a href="#">Digital comics</a>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- /footer top -->

            <!-- footer center -->
            <div class="footer-center">
                <div class="container">
                    <div class="footer-center-content">
                        <div class="col">
                            <ul>
                                <li><h3>dc comics</h3></li>
                                <li><a href="">characters</a></li>
                                <li><a href="">characters</a></li>
                                <li><a href="">characters</a></li>
                                <li><a href="">characters</a></li>
                            </ul>
                            <ul>
                                <li><h3>shop</h3></li>
                                <li><a href="">characters</a></li>

                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li><h3>dc</h3></li>
                                <li><a href="">characters</a></li>

                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li><h3>sites</h3></li>
                                <li><a href="">characters</a></li>

                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <!-- /footer center -->

            <!-- footer bottom -->
            <div class="footer-bottom">
                <div class="container">
                    <div class="sign-up">
                    <button>Sign-up now!</button>
                    </div>
                    <div class="social-bar"></div>
                </div>
            </div>
            <!-- /footer bottom -->
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang = "scss" scoped>
@import '../assets/style/partials/variables.scss';


    .footer-top {
        background-color: $secondaryColor;

        ul {
            height: 100%;
            display: flex;
            align-items: center;
            list-style: none;

            li {
                display: flex;
                align-items: center;
                margin: 0 20px;

                img {
                    width: 35px;
                }

                a {
                    text-decoration: none;
                    text-transform: uppercase;
                    font-size: .75rem;
                    color: $white;
                    margin-left: 10px;
                }
            }
        }
    }


    .footer-center {
        height: 300px;
        background-image: url('../assets/img/footer-bg.jpg');

        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            background-image: url('../assets/img/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: right;
            background-size: 40%;
                    }
    }


    .footer-center-content {
        display: flex;

        .col {
            margin-right: 30px;

            ul {
                list-style: none;

                li h3 {
                    text-transform: uppercase;
                    color: $white;
                        }

                li a {
                    color: $lightGray;
                    text-decoration: none;
                    font-size: .75rem;
                        }

                }
            }
    }


    .footer-bottom {
        background-color: $darkGray;

        .container {
            display: flex;
            padding: 20px 0;

            .sign-up button {
                background-color: $darkGray;
                color: $white;
                font-size: .9375rem;
                font-weight: 700;
                text-transform: uppercase;
                padding: 10px;
                border: 2px solid $secondaryColor;
                            }
                    }

    }


</style>