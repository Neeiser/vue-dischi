<template>
    <main>
        <div class="container d-flex justify-content-center flex-wrap py-3">
            <GridSpotify v-for="(artist, index) in arrArtists" 
            :key="index" 
            :artistData="artist">
            </GridSpotify>
        </div> 
    </main>
</template>

<script>
import GridSpotify from './GridSpotify.vue';
import axios from 'axios';

export default {
    name:'MainSpotify',
    data () {
        return{
            arrArtists: null,
        };
    },
    components:{
        GridSpotify,
    },
    created(){
        axios
        .get("https://flynn.boolean.careers/exercises/api/array/music")
        .then((item) => {
            this.arrArtists = item.data.response
            console.log(this.arrArtists)
        })
    }
}
</script>

<style scoped lang="scss">
@import "../assets/styles/partials/variables.scss";
main{
    background-color: $blueMain;
}
</style>
