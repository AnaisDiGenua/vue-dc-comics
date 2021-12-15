<template>
    <li>
        <a href="#">
            <img :src="socialLink.src" :alt="socialLink.name"/>
        </a>
    </li>
</template>

<script>
export default {
    name: "SocialLinks",
    props: {
        socialLink: Object
    }
};
</script>

<style lang = "scss" scoped>
@import '../../assets/style/partials/variables.scss';
            
    li {
        display: inline-block;
        margin: 0 10px;

        a img {
            width: 30px;
            }
    }
</style>