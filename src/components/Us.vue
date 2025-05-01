<template>
  <section class="why_section layout_padding">
    <div class="container">
      <div class="heading_container heading_center">
        <h2>Why Choose <span>Us</span></h2>
      </div>
      <div class="why_container">
        <cardus v-for="(item,index) in infor" :key="index" :name="item.name" :image="item.image"></cardus>
      </div>
      <div class="btn-box">
        <a href=""> Read More </a>
      </div>
    </div>
  </section>
</template>

<script>
    import cardus from "@/components/card/cardus.vue";

    export default{
        components:{
            cardus,
        },
        data(){
            return{
                infor:[
                    {name:"Expert Management",image:"images/w1.png"},
                    {name:"Secure Investment",image:"images/w2.png"},
                    {name:"Instant Trading",image:"images/w3.png"},
                    {name:"Happy Customers",image:"images/w4.png"},
                ]
            }
        }
        
    }
</script>
