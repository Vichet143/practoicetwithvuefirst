<template>
    <section class="team_section layout_padding">
    <div class="container-fluid">
      <div class="heading_container heading_center">
        <h2 class="">
          Our <span> Team</span>
        </h2>
      </div>

      <div class="team_container">
        <div class="row">
            <cardteam v-for="(item, index) in infor" 
            :key="index" 
            :name="item.name" 
            :image="item.image" 
            :skill="item.skill">
        </cardteam>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
    import cardteam from "@/components/card/cardteam.vue";

    export default{
        components:{
            cardteam,
        },
        data(){
            return{
                infor:[
                    {name:" Joseph Brown",image:"images/team-1.jpg",skill:"Marketing Head"},
                    {name:" Nancy White",image:"images/team-2.jpg",skill:"Marketing Head"},
                    {name:" Earl Martinez",image:"images/team-3.jpg",skill:"Marketing Head"},
                    {name:" Josephine Allard",image:"images/team-4.jpg",skill:"Marketing Head"},
                ]
            }
        }
    }
</script>