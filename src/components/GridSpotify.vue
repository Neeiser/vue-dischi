<template>
    <div>
        <div class="col-6 col-md-2">
            <img :src="artistData.poster" alt="">
            <h2>{{ artistData.title }}</h2>
            <span>{{ artistData.author }}</span>
            <span>{{ artistData.year }}</span>
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

</style>
