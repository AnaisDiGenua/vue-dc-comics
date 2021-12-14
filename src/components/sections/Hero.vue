<template>
    <section>
        <div class="hero">
            <img src="../../assets/img/jumbotron.jpg" alt="">
        </div>
    </section>
</template>

<script>
export default {
    name: 'Hero'
}
</script>

<style lang = "scss" scoped>
    section {
        height: 330px;

        .hero {
            height: 100%;

            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
    }
</style>