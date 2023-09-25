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
        <img class="jumbo_img" src="../assets/img/jumbotron.jpg" alt="">

        <div class="container">
            <div class="row row-cols-1 row-cols-sm-3 row-cols-md-4 row-cols-lg-6 py-4">
                <AppComics :thumb="comic.thumb" :series="comic.series" :type="comic.type" :price="comic.price"
                    v-for="comic in comics" />
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
</style>