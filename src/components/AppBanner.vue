<script>
export default {
    name: 'AppBanner'
}
</script>

<template>
    <div id="banner" class="d-flex align-items-center">
        <div class="wrapper container d-flex justify-content-around align-items-center">
            <a href="#" class="d-flex justify-content-center align-items-center">
                <img width="50" src="../assets/img/buy-comics-digital-comics.png" alt="">
                <div class="banner_text">digital comics</div>
            </a>
            <a href="#" class="d-flex justify-content-center align-items-center">
                <img width="50" src="../assets/img/buy-comics-merchandise.png" alt="">
                <div class="banner_text">dc merchandise</div>
            </a>
            <a href="#" class="d-flex justify-content-center align-items-center">
                <img width="50" src="../assets/img/buy-comics-subscriptions.png" alt="">
                <div class="banner_text">subscription</div>
            </a>
            <a href="#" class="d-flex justify-content-center align-items-center">
                <img width="50" src="../assets/img/buy-comics-shop-locator.png" alt="">
                <div class="banner_text">comic shop locator</div>
            </a>
            <a href="#" class="d-flex justify-content-center align-items-center">
                <img width="50" src="../assets/img/buy-dc-power-visa.svg" alt="">
                <div class="banner_text">dc power visa</div>
            </a>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/viariables' as *;
#banner {
    background-color: $dc_primary;
    height: 150px;
    .wrapper {
        height: 55px;
        a {
            text-decoration: none;
            img {
                height: 55px;
                object-fit: scale-down;
            }
            .banner_text {
                color: white;
                text-transform: uppercase;
                font-size: 0.8rem;
            }
        }
    }
}
</style>