<template>
    <footer>
            <!-- footer top -->
            <div class="footer-top">
                <div class="container">
                    <ul>
                        <Shop v-for="(shopLink,index) in shopLinks" :shop-link="shopLink" :key="index"/>
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
            <SocialBar/>
            <!-- /footer bottom -->
    </footer>
</template>


<script>
import Shop from '../sections/Shop.vue';
import FooterLinks from '../sections/FooterLinks.vue';
import SocialBar from '../sections/SocialBar.vue';

export default {
    name: 'Footer',
    components: {
        Shop,
        FooterLinks,
        SocialBar
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
            justify-content: center;
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



</style>