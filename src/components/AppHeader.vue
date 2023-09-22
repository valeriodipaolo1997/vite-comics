<script>
export default {
    name: 'AppHeader'
}
</script>

<template>
    <header>
        <div class="header_wrapper container d-flex justify-content-between align-items-center w-75">


            <img width="75" src="../assets/img/dc-logo.png" alt="">


            <div>
                <nav class="navbar navbar-expand navbar-light">
                    <ul class="nav navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link active" href="#" aria-current="page">characters</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">comics</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">movies</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">tv</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">games</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">collectibles</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">videos</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">fans</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">news</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#">shop</a>
                        </li>
                    </ul>
                </nav>
            </div>

        </div>
    </header>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/viariables' as *;
header {
    height: 120px;
    .header_wrapper {
        height: 100%;
        li {
            a {
                text-transform: uppercase;
                &.active {
                    color: $dc_primary;
                }
            }
            & a.active {
                border-bottom: 2px solid $dc_primary;
            }
        }
    }
}
</style>