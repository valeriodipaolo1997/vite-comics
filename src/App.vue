<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppBanner from './components/AppBanner.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return {
    }
  },
  components: {
    AppHeader,
    AppJumbotron,
    AppBanner,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppJumbotron />
  <AppBanner />
  <AppFooter />
</template>
<style lang="scss"></style>
