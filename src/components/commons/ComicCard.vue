<template>
    <div class="comic">
        <img :src="comic.thumb" :alt="comic.series">
        <h3>{{comic.series}}</h3>
    </div>
</template>

<script>
export default {
    name: 'ComicCard',
    props: {
        comic: Object
    }
}
</script>

<style lang = "scss" scoped>
    .comic {
        width: calc(100% / 6 - 40px); /*DEBUG*/
        margin: 20px;

        h3 {
            font-size: .875rem;
            font-weight: 400;
        }

        img {
            width: 100%;
            height: 160px;
            object-fit: cover;
            object-position: top;
        }
    }
</style>