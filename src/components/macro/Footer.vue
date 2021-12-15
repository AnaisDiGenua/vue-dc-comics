<template>
    <footer>

        <FooterTop/>

        <FooterCenter/>

        <FooterBottom/>

    </footer>
</template>


<script>
import FooterTop from '../sections/FooterTop.vue';
import FooterCenter from '../sections/FooterCenter.vue';
import FooterBottom from '../sections/FooterBottom.vue';

export default {
    name: 'Footer',
    components: {
        FooterTop,
        FooterCenter,
        FooterBottom
    }
}
</script>


<style lang = "scss" scoped>

</style>