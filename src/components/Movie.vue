<template>
    <div class="container1">
        <div class="flex2">
            <cardmovie v-for="(item,index) in movie" :key="index"
            :image="item.image.medium"
            :name="item.name"
            :languge="item.language"
            :type="item.genres"></cardmovie>
        </div>
    </div>
</template>

<script>
import axios from "axios";
import cardmovie from "./card/cardmovie.vue";

    export default{
        components:{
            cardmovie,
        },
        data(){
            return{
                movie:[]
            };
        },
        beforeCreate(){

        },
        async created(){
            const respones = await axios.get("https://api.tvmaze.com/search/shows?q=girls")
            console.log(respones.data);
            this.movie = respones.data.map(item => item.show);
            
        },
    }
</script>