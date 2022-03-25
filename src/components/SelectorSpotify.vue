<template>
    <option value="artistGenre.genre">{{ artistGenre.genre }}</option>
</template>

<script>


export default {
    name:'SelectorSpotify',
    props: {
        artistGenre: Object,
    }
}
</script>

<style scoped lang="scss">

</style>
