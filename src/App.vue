<template>
  <Navbar></Navbar>
  <Servies></Servies>
  <About></About>
  <Us></Us>
  <Team></Team>
  <Allcourse></Allcourse>
</template>

<script>
  import Navbar from "@/components/Nav.vue";
  import Servies from "@/components/Servies.vue";
  import About from "@/components/About.vue";
  import Us from "@/components/Us.vue";
  import Team from "@/components/Team.vue";
  import Allcourse from "@/components/Allcourse.vue";
  
  export default {
    components: {
      Navbar,
      Servies,
      About,
      Us,
      Team,
      Allcourse,
    },
  };
</script>

