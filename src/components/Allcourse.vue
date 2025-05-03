<template>
  <div class="container1">
    <div class="flex">
        <cardcourse v-for="(item , index) in coures" 
        :key="index"
        :image="item.image"
        :name="item.name"
        :namefooter="item.title"
        :txtcard="item.shortDescription"
        :price="item.price"
        :time="item.updatedDate"></cardcourse>
    </div>
  </div>
</template>

<script>
import cardcourse from './card/cardcourse.vue';
 import axios from 'axios';
    export default{
        beforeCreate(){
      console.log("hell");
      
    },
    components:{
        cardcourse,
    },
    data(){
        return{
            coures:[{image:"images/html.jpg",name:"DevOps"},{image:"images/linux.jpg",name:"Web Development"}],
        }
    },
    async created(){
      const respones = await axios.get("/v1/courses");
      console.log(respones.data);
      
      this.coures = respones.data;
    },
    }
</script>