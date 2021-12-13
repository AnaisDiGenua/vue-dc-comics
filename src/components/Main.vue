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

    .container {
        height: 100px; /*DEBUG*/
        background: $black; /*DEBUG*/
        color: $white; /*DEBUG*/
    }
</style>