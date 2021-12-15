<template>
    <footer>
            <!-- footer top -->
            <div class="footer-top">
                <div class="container">
                    <ul>
                        <ShopLinks v-for="(shopLink,index) in shopLinks" :shop-link="shopLink" :key="index"/>
                    </ul>
                </div>
            </div>
            <!-- /footer top -->

            <!-- footer center -->
            <div class="footer-center">
                <div class="container">
                    <FooterLinks/>
                </div>
            </div>
            <!-- /footer center -->

            <!-- footer bottom -->
            <div class="footer-bottom">
                <div class="container">
                    <div class="sign-up-cta">
                        <button>Sign-up now!</button>
                    </div>

                    <div class="social-box">
                        <div class="follow-us-cta">
                            <p>Follow us</p>
                        </div>
                        <div class="social-list">
                            <ul>
                                <SocialLinks v-for="(socialLink,index) in socialLinks" :social-link="socialLink" :key="index"/>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <!-- /footer bottom -->
    </footer>
</template>


<script>
import ShopLinks from '../sections/ShopLinks.vue';
import FooterLinks from '../sections/FooterLinks.vue';
import SocialLinks from '../sections/SocialLinks.vue';

export default {
    name: 'Footer',
    components: {
        ShopLinks,
        FooterLinks,
        SocialLinks
    },
    data() {
        return {
            // array del shop 
            shopLinks: [
                {
                    "src": require("../../assets/img/buy-comics-digital-comics.png"),
                    "name": "digital comics"
                },
                {
                    "src": require("../../assets/img/buy-comics-merchandise.png"),
                    "name": "dc merchandise"
                },
                {
                    "src": require("../../assets/img/buy-comics-subscriptions.png"),
                    "name": "subscription"
                },
                {
                    "src": require("../../assets/img/buy-comics-shop-locator.png"),
                    "name": "comic shop locator"
                },
                {
                    "src": require("../../assets/img/buy-dc-power-visa.svg"),
                    "name": "dc power visa"
                },
            ],
            socialLinks: [
                {
                    "src": require("../../assets/img/footer-facebook.png"),
                    "name": "facebook link"
                },
                {
                    "src": require("../../assets/img/footer-twitter.png"),
                    "name": "twitter link"
                },
                {
                    "src": require("../../assets/img/footer-youtube.png"),
                    "name": "youtube link"
                },
                {
                    "src": require("../../assets/img/footer-pinterest.png"),
                    "name": "pinterest link"
                },
                {
                    "src": require("../../assets/img/footer-periscope.png"),
                    "name": "periscope link"
                },
            ]
        }
    }
}
</script>


<style lang = "scss" scoped>
@import '../../assets/style/partials/variables.scss';

    .footer-top {
        background-color: $secondaryColor;

        ul {
            height: 100%;
            display: flex;
            justify-content: space-around;
            align-items: center;
            list-style: none;
        }
    }

    .footer-center {
        background-image: url('../../assets/img/footer-bg.jpg');

        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            background-image: url('../../assets/img/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: right;
            background-size: 40%;
                    }
    }

    .footer-bottom {
        background-color: $darkGray;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;

            .sign-up-cta button {
                background-color: $darkGray;
                color: $white;
                font-size: .9375rem;
                font-weight: 700;
                text-transform: uppercase;
                padding: 10px;
                border: 2px solid $secondaryColor;
                cursor: pointer;
            }
        }
    }

    .social-box {
        display: flex;
        align-items: center;

        .follow-us-cta {
            margin-right: 20px;

            p {
                font-size: 1.25rem;
                text-transform: uppercase;
                font-weight: 700;
                color: $secondaryColor;
            }
        }

        .social-list ul {
            list-style: none;
        }
    }



</style>