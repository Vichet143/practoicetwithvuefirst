<template>
  <div class="col1">
    <div class="div">
      <div class="boximg">
        <img class="img-s" :src="image" alt="" />
      </div>
    </div>
    <h2 class="namemovie">{{ name }}</h2>
    <p class="lang">Languge:{{ languge }}</p>
    <p class="type">Type: {{ type }}</p>
  </div>
</template>

<script>

    export default{
        props:["image","name","languge","type"]
    }
</script>