<template>
    <main>
        <Hero/>
        <div class="container">
            <Comics/>
        </div>
    </main>
</template>

<script>
import Comics from '../sections/Comics.vue';
import Hero from '../sections/Hero.vue';

export default {
    name: 'Main',
    components: {
        Comics,
        Hero
    }
}
</script>

<style lang= "scss" scoped>
@import '../../assets/style/partials/variables.scss';
    main {
        background-color: $darkColor;
    }
</style>