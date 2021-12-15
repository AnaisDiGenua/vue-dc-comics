<template>
    <li>
        <img :src="shopLink.src" :alt="shopLink.name" />
        <a href="#">{{shopLink.name}}</a>
    </li>
</template>

<script>
export default {
    name: "ShopLinks",
    props: {
        shopLink: Object
    }
};
</script>

<style lang = "scss" scoped>
@import '../../assets/style/partials/variables.scss';

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
                font-size: .75rem;
                color: $white;
                margin-left: 10px;
                }
            }

</style>