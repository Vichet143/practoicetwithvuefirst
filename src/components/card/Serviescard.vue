<template>
    <div class="col-md-4">
            <div class="box">
              <div class="img-box">
                <img :src="image" alt="" />
              </div>
              <div class="detail-box">
                <h5>{{name}}</h5>
                <p>
                  fact that a reader will be distracted by the readable content
                  of a page when looking at its layout. The point of using
                </p>
                <a href=""> Read More </a>
              </div>
            </div>
          </div>
</template>

<script>
    export default{
        props:["name","image"],
    }
</script>