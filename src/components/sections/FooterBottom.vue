<template>
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
                        <li v-for="(socialLink, index) in socialLinks"
                            :key="index"
                        >
                            <a href="#">
                                <img :src="socialLink.src" :alt="socialLink.name" />
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            
        </div>
    </div>
</template>


<script>
export default {
    name: "FooterBottom",
    data() {
        return {
        socialLinks: [
            {
            src: require("../../assets/img/footer-facebook.png"),
            name: "facebook link",
            },
            {
            src: require("../../assets/img/footer-twitter.png"),
            name: "twitter link",
            },
            {
            src: require("../../assets/img/footer-youtube.png"),
            name: "youtube link",
            },
            {
            src: require("../../assets/img/footer-pinterest.png"),
            name: "pinterest link",
            },
            {
            src: require("../../assets/img/footer-periscope.png"),
            name: "periscope link",
            },
        ],
        };
    },
};
</script>


<style lang = "scss" scoped>
@import "../../assets/style/partials/variables.scss";

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

            li {
                display: inline-block;
                margin: 0 10px;

                a img {
                    width: 30px;
                }
            }
        }
    }
</style>