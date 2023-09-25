<script>
import AppComics from './AppComics.vue';
import comics from '../dc-comics';

export default {
    name: 'AppJumbotron',
    data() {
        return {
            comics: comics
        }
    },
    components: {
        AppComics,
    }

}
</script>

<template>
    <div id="jumbo">
        <div>
            <img class="jumbo_img" src="../assets/img/jumbotron.jpg" alt="">
            <div class="container position-relative">
                <div class="current_btn">
                    <a href="##" class="btn btn-primary rounded-0 text-uppercase px-5 fs-5 fw-bolder">current series</a>
                </div>
            </div>
        </div>

        <div class="container py-4">

            <div class="row row-cols-1 row-cols-sm-3 row-cols-md-4 row-cols-lg-6 py-4">
                <AppComics :thumb="comic.thumb" :series="comic.series" :type="comic.type" :price="comic.price"
                    v-for="comic in comics" />
            </div>

            <div class="text-center py-4">
                <a href="##" class="btn btn-primary rounded-0 text-uppercase px-5">load more</a>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/viariables' as *;

#jumbo {

    background-color: $dc_darker;
}

.jumbo_img {
    height: 400px;
    width: 100%;
    object-fit: cover;
    object-position: top;
}

.current_btn {
        position: absolute;
        bottom: 0;
        left: -0.5rem;
        transform: translatey(50%);
    }

</style>