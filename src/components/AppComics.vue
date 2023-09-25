<script>
export default {
    name: 'AppComics',
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String
    },
    data() {
        return {
        }
    }
}
</script>

<template>
    <div class="col pt-4">
        <div class="card">
            <img class="card-img-top" :src="thumb" alt="">
            <div class="card-body ps-0">
                <h6 class="card-title text-white text-uppercase"> {{ series }}</h6>
            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    background-color: transparent;
    img {
        height: 185px;
        object-fit: cover;
        object-position: top;
    }
    h6 {
        font-size: 0.9rem;
    }
}
</style>