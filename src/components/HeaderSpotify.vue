<template>
    <header>
        <div class="container-fluid p-4 d-flex justify-content-between align-items-center">
            <img class="col-6 img-fluid" src="../assets/img/spotify-logo.png" alt="">
            <SelectorSpotify></SelectorSpotify>
        </div>
    </header>
</template>

<script>
import SelectorSpotify from './SelectorSpotify.vue'

export default {
    name:'HeaderSpotify',
    components:{
        SelectorSpotify,
    }
}
</script>

<style scoped lang="scss">
@import "../assets/styles/partials/variables.scss";

header{
    background-color: $grayBlue;
    img{
        height: 50px;
        width: 50px;
    };
}

</style>