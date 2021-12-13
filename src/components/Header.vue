<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo pagina dc">
            </div>
            <nav>
                <ul>
                    <li><a href="">Characters</a></li>
                    <li><a href="" class="active">Comics</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang = "scss" scoped>
@import '../assets/style/partials/variables.scss';

    header {
        height: 100px;

            .container {
                height: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                        .logo img {
                            width: 80px;
                        }
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