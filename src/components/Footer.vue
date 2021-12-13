<template>
    <footer>
        <div class="container">
            <!-- footer top -->
            <div class="footer-top">
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
            <!-- /footer top -->

            <!-- footer center -->
            <div class="footer-center"></div>
            <!-- /footer center -->

            <!-- footer bottom -->
            <div class="footer-bottom"></div>
            <!-- /footer bottom -->
        </div>
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
        height: 100px; /*debug*/

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

</style>