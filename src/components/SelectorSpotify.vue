<template>
    <div>
        <select class="p-1" name="genre-selector" id="genre-selector">
            <option value=""></option>
            <option value="Rock">Rock</option>
            <option value="Pop">Pop</option>
            <option value="Jazz">Jazz</option>
            <option value="Metal">Metal</option>
        </select>
    </div>
</template>

<script>


export default {
    name:'SelectorSpotify'
}
</script>

<style scoped lang="scss">
@import "../assets/styles/partials/variables.scss";

select{
    width: 100px;
}

</style>
