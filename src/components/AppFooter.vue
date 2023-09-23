<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
    <footer>

        <div class="main_footer">
            <div class="container">
                <div class="row">
                    <div class="col-6 py-5">
                        <div class="d-flex gap-5">

                            <div>
                                <h3>dc comics</h3>
                                <ul class="list-unstyled">
                                    <li>
                                        <a href="#">Characters</a>
                                    </li>
                                    <li>
                                        <a href="#">Comics</a>
                                    </li>
                                    <li>
                                        <a href="#">Movies</a>
                                    </li>
                                    <li>
                                        <a href="#">TV</a>
                                    </li>
                                    <li>
                                        <a href="#">Games</a>
                                    </li>
                                    <li>
                                        <a href="#">Videos</a>
                                    </li>
                                    <li>
                                        <a href="#">News</a>
                                    </li>
                                </ul>


                                <h3>shop</h3>
                                <ul class="list-unstyled">
                                    <li>
                                        <a href="#">Shop DC</a>
                                    </li>
                                    <li>
                                        <a href="#">Shop DC Collectibles</a>
                                    </li>
                                </ul>
                            </div>

                            <div>
                                <h3>dc</h3>
                                <ul class="list-unstyled">
                                    <li>
                                        <a href="#">Terms Of Use</a>
                                    </li>

                                    <li>
                                        <a href="#">Privacy policy (New)</a>
                                    </li>

                                    <li>
                                        <a href="#">Ad Choices</a>
                                    </li>

                                    <li>
                                        <a href="#">Advertising</a>
                                    </li>

                                    <li>
                                        <a href="#">Jobs</a>
                                    </li>

                                    <li>
                                        <a href="#">Subscriptions</a>
                                    </li>

                                    <li>
                                        <a href="#">Talent Workshops</a>
                                    </li>

                                    <li>
                                        <a href="#">CPSC Certificates</a>
                                    </li>

                                    <li>
                                        <a href="#">Ratings</a>
                                    </li>

                                    <li>
                                        <a href="#">Shop Help</a>
                                    </li>

                                    <li>
                                        <a href="#">Contact US</a>
                                    </li>

                                </ul>
                            </div>

                            <div>
                                <h3>sites</h3>
                                <ul class="list-unstyled">
                                    <li>
                                        <a href="#">DC</a>
                                    </li>
                                    <li>
                                        <a href="#">MAD Magazine</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Kids</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Universe</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Power Visa</a>
                                    </li>
                                </ul>
                            </div>

                        </div>
                    </div>
                    <div class="col-6 logo_dc">

                    </div>
                </div>
            </div>
        </div>

        <div class="footer_bottom">
            <div class="container d-flex justify-content-between h-100">

                <div class="bottom_left d-flex align-items-center">
                    <a href="##">
                        <button class="btn btn-outline-primary text-white rounded-0 fs-5">
                            SIGN-UP NOW!
                        </button>
                    </a>
                </div>

                <div class="bottom_right d-flex align-items-center gap-4">
                    <h3>FOLLOW US</h3>
                    <a href="##">
                        <img src="../assets/img/footer-facebook.png" alt="">
                    </a>
                    <a href="##">
                        <img src="../assets/img/footer-twitter.png" alt="">
                    </a>
                    <a href="##">
                        <img src="../assets/img/footer-youtube.png" alt="">
                    </a>
                    <a href="##">
                        <img src="../assets/img/footer-pinterest.png" alt="">
                    </a>
                    <a href="##">
                        <img src="../assets/img/footer-periscope.png" alt="">
                    </a>
                </div>


            </div>


        </div>

        

    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/viariables' as *;

.main_footer {
    height: 400px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;

    h3 {
        text-transform: uppercase;
        color: white;
        font-weight: bolder;
        font-size: 1.25rem;
    }

    a {
        color: gray;
        text-decoration: none;
    }

    .logo_dc {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center;
    }
}

.footer_bottom {
    height: 110px;
    background-color: $dc_dark;

    h3 {
        color: $dc_primary;
        font-weight: bold;
        font-size: 1.25rem;
        padding-top: 0.5rem;
    }
}</style>