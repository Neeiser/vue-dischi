<template>
    <main>
        <div class="container">
            
        </div> 
    </main>
</template>

<script>
import axios from 'axios';

export default {
    name:'MainSpotify',
     data () {
        return{
            arrChar:[],
        }
    },
    created(){
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then(function(response) {
            this.arrChar = response.data.response
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
