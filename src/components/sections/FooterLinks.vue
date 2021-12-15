<template>
    <div class="footer-center">
        <div class="container">
            <div class="footer-center-content">
                <div class="col">
                    <ul>
                        <li>
                            <h3>dc comics</h3>
                        </li>
                        <li>
                            <a href="">characters</a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <h3>shop</h3>
                            </li>
                        <li>
                            <a href="">characters</a>
                        </li>
                    </ul>
                </div>

                <div class="col">
                    <ul>
                        <li>
                            <h3>dc</h3>
                        </li>
                        <li>
                            <a href="">characters</a>
                        </li>
                    </ul>
                </div>

                <div class="col">
                    <ul>
                        <li>
                            <h3>sites</h3>
                        </li>
                        <li>
                            <a href="">characters</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterLinks",
};
</script>

<style lang = "scss" scoped>
@import '../../assets/style/partials/variables.scss';

    .footer-center {
        height: 300px;
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


    .footer-center-content {
        display: flex;

        .col {
            margin-right: 30px;

            ul {
                list-style: none;
                margin-bottom: 15px;

                li h3 {
                    font-size: 1.25rem;
                        }

                li a {
                    font-size: .8125rem;
                    color: $lightGray;
                    text-decoration: none;
                    }

                }
            }
    }
</style>