<template>
    <div class="footer-top">
        <div class="container">
            <ul>
                <li v-for="(shopLink,index) in shopLinks" :key="index" >
                    <img :src="shopLink.src" :alt="shopLink.name" />
                    <a href="#">{{shopLink.name}}</a>
                </li>
            </ul>
        </div>
    </div>
</template>


<script>
export default {
    name: "FooterTop",
    data() {
        return {
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
        }
    }
};
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

            li {
                display: flex;
                align-items: center;

                img {
                    width: 35px;
                    cursor: pointer;
                    }

                    a {
                        text-decoration: none;
                        text-transform: uppercase;
                        font-size: .9375rem;
                        color: $white;
                        margin-left: 10px;
                        }
                    }
        }
    }


</style>