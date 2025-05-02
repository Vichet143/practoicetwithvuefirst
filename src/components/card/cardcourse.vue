<template>
    <div class="col-">
        <div class="allimg">
          <div class="box-img">
            <img class="img-s" :src="image" alt="" />
          </div>
        </div>
        <div class="alltext" style="margin-top: 10px">
          <h1 style="color: #9ca3af; font-size: 18px;margin-top: 30px;">{{ name }}</h1>
          <h1 style="font-size: 20px">{{ namefooter }}</h1>
          <p>{{ txtcard }}</p>
          <div class="cardfooter">
            <button class="re">Register</button>
            <div style="display: flex;color: #9ca3af">
              <p class="prize">${{price}}</p>
              <p>|</p>
              <i style="margin: 5px 10px;" class="fa-solid fa-clock"></i>
              <p style="margin-left: 10px;margin-top: 2px;">{{ time }}</p>
            </div>
          </div>
        </div>
      </div>
</template>

<script>
    export default{
        props:["image","name","namefooter","txtcard","price","time"]
    }
</script>