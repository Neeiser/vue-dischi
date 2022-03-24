<template>
    <div class="col-2 col-md-2">
        <img :src="artistData.poster" alt="">
        <h2>{{ artistData.title }}</h2>
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
img{
    width: 100px;
}
</style>
