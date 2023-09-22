<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppBanner from './components/AppBanner.vue';

export default {
  data() {
    return {
    }
  },
  components: {
    AppHeader,
    AppJumbotron,
    AppBanner
  }
}
</script>

<template>
  <AppHeader />
  <AppJumbotron />
  <AppBanner />
</template>
<style lang="scss"></style>
