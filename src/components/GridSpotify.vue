<template>
    <div class="d-flex artist-box m-3">
        <div class="d-flex flex-column align-items-center justify-content-around artist-item">
            <section class="artist-top p-3">
                <img class="img-fluid pb-3" :src="artistData.poster" alt="">
                <h2 class="text-center fs-5 text-white">{{ artistData.title.toUpperCase() }}</h2>
            </section>
            <section class="d-flex align-items-center flex-column artist-bottom mb-3">
                <span class="text-secondary justify-self-end">{{ artistData.author }}</span>
                <span class="text-secondary justify-self-end">{{ artistData.year }}</span>
            </section>
        </div>
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
    .artist-item{
        width: 200px;
    }
}
</style>
