<template>
    <div class="footer-center-content">
        <div class="col">
            <ul>
                <li>
                    <h3>dc comics</h3>
                </li>
                <li>
                    <a href="#">Characters</a>
                </li>
                <li>
                    <a href="#">Comics</a>
                </li>
                <li>
                    <a href="#">Movies</a>
                </li>
                <li>
                    <a href="#">TV</a>
                </li>
                <li>
                    <a href="#">Games</a>
                </li>
                <li>
                    <a href="#">Videos</a>
                </li>
                <li>
                    <a href="#">News</a>
                </li>
            </ul>
            <ul>
                <li>
                    <h3>shop</h3>
                </li>
                <li>
                    <a href="#">Shop DC</a>
                </li>
                <li>
                    <a href="#">Shop DC Collectibles</a>
                </li>
            </ul>
        </div>

        <div class="col">
            <ul>
                <li>
                    <h3>dc</h3>
                </li>
                <li>
                    <a href="#">Terms of use</a>
                </li>
                <li>
                    <a href="#">Privacy policy(New)</a>
                </li>
                <li>
                    <a href="#">Ad Choises</a>
                </li>
                <li>
                    <a href="#">Advertising</a>
                </li>
                <li>
                    <a href="#">Jobs</a>
                </li>
                <li>
                    <a href="#">Subscriptions</a>
                </li>
                <li>
                    <a href="#">Talent Workshops</a>
                </li>
                <li>
                    <a href="#">Terms of use</a>
                </li>
                <li>
                    <a href="#">CPSC Certicates</a>
                </li>
                <li>
                    <a href="#">Ratings</a>
                </li>
                <li>
                    <a href="#">Shop Help</a>
                </li>
                <li>
                    <a href="#">Contact us</a>
                </li>
            </ul>
        </div>

        <div class="col">
            <ul>
                <li>
                    <h3>sites</h3>
                </li>
                <li>
                    <a href="#">DC</a>
                </li>
                <li>
                    <a href="#">MAD Mad Magazines</a>
                </li>
                <li>
                    <a href="#">DC Kids</a>
                </li>
                <li>
                    <a href="#">DC Universe</a>
                </li>
                <li>
                    <a href="#">DC Power Visa</a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterLinks",
};
</script>

<style lang = "scss" scoped>
@import "../../assets/style/partials/variables.scss";

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
            font-size: 0.8125rem;
            color: $lightGray;
            text-decoration: none;
        }
        }
    }
}
</style>