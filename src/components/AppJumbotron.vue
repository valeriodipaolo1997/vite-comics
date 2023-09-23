<script>
export default {
    name: 'AppJumbotron'
}
</script>

<template>
    <div id="jumbo"> 
     <div class="container pt-5">
        <h3 class="text-white"> Content goes here </h3>
     </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/viariables' as *;
#jumbo {
   height: 150px; 
    background-color: black;
}
</style>