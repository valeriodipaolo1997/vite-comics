<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            activeLink: 0,
            navItems: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop']
        }
    }
}
</script>

<template>
    <header>
        <div class="header_wrapper container d-flex justify-content-between align-items-center w-75">


            <img width="75" src="../assets/img/dc-logo.png" alt="">


            <div>
                <nav class="navbar navbar-expand navbar-light">
                    <ul v-for="(item, index) in navItems" class="nav navbar-nav">
                        <li class="nav-item" @click="activeLink = index">
                            <a class="nav-link" :class="activeLink === index ? 'active' : ''" href="#"
                                aria-current="page">{{ item }}</a>
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