<template>
  <section class="service_section layout_padding">
    <div class="service_container">
      <div class="container">
        <div class="heading_container heading_center">
          <h2>Our <span>Services</span></h2>
          <p>
            There are many variations of passages of Lorem Ipsum available, but
            the majority have suffered alteration
          </p>
        </div>
        <div class="row">
          <Serviescard v-for="(item,index) in servies" 
            :key="index" 
            :name="item.name"
            :image="item.image">
            
          </Serviescard>
        </div>
        <div class="btn-box">
          <a href=""> View All </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Serviescard from "@/components/card/Serviescard.vue";

export default {
  components: {
    Serviescard,
  },
  data() {
    return {
      servies: [
        { name: "Currency Wallet", image: "images/s1.png" },
        { name: "Security Storage", image: "images/s2.png" },
        { name: "Expert Support", image: "images/s3.png" },
      ],
    };
  },
};
</script>