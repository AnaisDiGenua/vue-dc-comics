<template>
    <main>
        <div class="container">
            <Comics/>
        </div>
    </main>
</template>

<script>
import Comics from '../sections/Comics.vue';

export default {
    name: 'Main',
    components: {
        Comics
    }
}
</script>

<style lang= "scss" scoped>
@import '../../assets/style/partials/variables.scss';
    main {
        background-color: $darkColor;
    }
</style>