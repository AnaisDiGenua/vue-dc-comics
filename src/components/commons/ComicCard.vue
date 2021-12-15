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

        h3 {
            font-size: .9375rem;
            font-weight: 400;
            margin-top: 10px;
        }

        img {
            width: 100%;
            height: 160px;
            object-fit: cover;
            object-position: top;
        }
    }
</style>