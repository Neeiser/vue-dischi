<template>
    <div class="d-flex flex-column align-items-center col-6 col-md-3 artist-box m-3">
        <img class="img-fluid" :src="artistData.poster" alt="">
        <h2 class="text-center">{{ artistData.title }}</h2>
        <span>{{ artistData.author }}</span>
        <span>{{ artistData.year }}</span>
    </div>
</template>

<script>

export default {
    name:'GridSpotify',
    props: {
        artistData: Object,
    },
}

</script>

<style scoped lang="scss">
@import "../assets/styles/partials/variables.scss";

.artist-box{
    background-color: $grayBlue;
    img{
        height: 200px;
    }
}
</style>
