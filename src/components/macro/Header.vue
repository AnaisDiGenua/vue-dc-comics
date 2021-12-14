<template>
    <header>
        <div class="container">
            <Logo/>
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index"><a :class="{active: link.current}" :href="link.url">{{link.text}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
import Logo from '../commons/Logo.vue';

export default {
    name: 'Header',
    components: {
        Logo
    },
    data() {
        return {
            // array link nav
            links: [
                {
                    text: "Characters",
                    url: "#",
                    current: false
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false
                },
                {
                    text: "Games",
                    url: "#",
                    current: false
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false
                },
                {
                    text: "News",
                    url: "#",
                    current: false
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false
                }
            ]
        }
    }
}
</script>

<style lang = "scss" scoped>
@import '../../assets/style/partials/variables.scss';

    header {
        height: 100px;

            .container {
                height: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;
                padding: 0;
            }
    }


    nav {
        text-align: right;

        ul {
            list-style: none;

            li {
                display: inline-block;

                a {
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: 700;
                    padding: 0 15px;
                    color: $darkGray;

                    &.active, &:hover {
                        color: $secondaryColor;
                    }
                }
            }
        }
    }
</style>