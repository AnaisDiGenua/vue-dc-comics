<template>
    <header>
        <div class="container">
            <Logo/>
            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index" @click="selectLink(index)"><a :class="currentLink == index ? 'active' : '' " :href="link.url">{{link.text}}</a></li>
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
                },
                {
                    text: "Comics",
                    url: "#",
                },
                {
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "Tv",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Collectibles",
                    url: "#",
                },
                {
                    text: "Videos",
                    url: "#",
                },
                {
                    text: "Fans",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",
                },
                {
                    text: "Shop",
                    url: "#",
                }
            ],
            currentLink: 0
        }
    },
    methods: {
        selectLink(index) {
            this.currentLink = index;
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
                    padding: 34px 15px;
                    color: $darkGray;

                    &.active, &:hover {
                        color: $secondaryColor;
                        border-bottom: 5px solid $secondaryColor;
                    }
                }
            }
        }
    }
</style>