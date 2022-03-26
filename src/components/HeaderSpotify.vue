<template>
    <header>
        <div class="container-fluid p-4 d-flex justify-content-between align-items-center">
            <img class="col-6 img-fluid" src="../assets/img/spotify-logo.png" alt="">
            <select v-show="showSelector" class="p-1" name="genre-selector" id="genre-selector">
                <option value=""></option>
                <SelectorSpotify v-for="(itemGenre, index) in arrGenre" 
                :key="index"
                :artistGenre="itemGenre">
                </SelectorSpotify>
            </select>
        </div>
    </header>
</template>

<script>
import SelectorSpotify from './SelectorSpotify.vue'
import axios from 'axios';

export default {
    name:'HeaderSpotify',
    data () {
        return{
            arrGenre: null,
            showSelector: false,
        };
    },
    components:{
        SelectorSpotify,
    },
    created(){
        axios
        .get("https://flynn.boolean.careers/exercises/api/array/music")
        .then((item) => {
            this.arrGenre = item.data.response;
            this.arrGenre.forEach((ele, index) => {
                if (this.arrGenre.item == this.arrGenre.item){
                    this.arrGenre.splice(ele, index);
                }
            });
                console.log(this.arrGenre)
        }),
        setTimeout(()=>{
            this.showSelector = true;
        }, 2000)
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
    }
    select{
    width: 100px;
    }
}

</style>