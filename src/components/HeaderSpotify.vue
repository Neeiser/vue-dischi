<template>
    <header>
        <div class="container-fluid p-4 d-flex justify-content-between align-items-center">
            <img class="col-6 img-fluid" src="../assets/img/spotify-logo.png" alt="">
            <select class="p-1" name="genre-selector" id="genre-selector">
                <option value=""></option>
                <option value="Rock">Rock</option>
                <option value="Pop">Pop</option>
                <option value="Jazz">Jazz</option>
                <option value="Metal">Metal</option>
            </select>
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

header{
    --bs-gutter-x: 0rem; /* mi dava problemi di render */
    background-color: $grayBlue;
    img{
        height: 50px;
        width: 50px;
    };
    select{
        width: 100px;
    }
}

</style>