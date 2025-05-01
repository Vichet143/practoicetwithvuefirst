<template>
  <Navbar></Navbar>
  <Servies></Servies>
  <About></About>
  <Us></Us>
  <Team></Team>
</template>

<script>
  import Navbar from "@/components/Nav.vue";
  import Servies from "@/components/Servies.vue";
  import About from "@/components/About.vue";
  import Us from "@/components/Us.vue";
  import Team from "@/components/Team.vue";
  
  export default {
    components: {
      Navbar,
      Servies,
      About,
      Us,
      Team,
    },
  };
</script>

