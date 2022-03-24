<template>
    <header class="row">
        <div class="container p-4 d-flex justify-content-between align-items-center">
            <img class="col-6 img-fluid" src="../assets/img/spotify-logo.png" alt="">
            <span class="col-2">Dropdown goes here</span>
        </div>
    </header>
</template>

<script>
export default {
    name:'HeaderSpotify',
}
</script>

<style scoped lang="scss">
@import "../assets/styles/partials/variables.scss";

.row{
    --bs-gutter-x: 0rem; /* mi dava problemi di render */
    background-color: $grayBlue;
    img{
        height: 50px;
        width: 50px;
    };
    span{
        color: white;
    }
}

</style>