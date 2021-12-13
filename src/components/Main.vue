<template>
    <main>
        <div class="container">
            Content goes here
        </div>
    </main>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style lang= "scss" scoped>
@import '../assets/style/partials/variables.scss';
    main {
        height: 100px; /*DEBUG*/
        background: $black; /*DEBUG*/
    }
    .container {
        color: $white; /*DEBUG*/
    }
</style>