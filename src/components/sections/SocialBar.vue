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
                        <li>
                            <a href="#">
                                <img src="../../assets/img/footer-facebook.png" alt="" />
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../../assets/img/footer-facebook.png" alt="" />
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../../assets/img/footer-facebook.png" alt="" />
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
    name: "SocialBar",
};
</script>

<style lang = "scss" scoped>
@import '../../assets/style/partials/variables.scss';

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