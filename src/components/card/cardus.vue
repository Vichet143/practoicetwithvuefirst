<template>
    <div class="box">
          <div class="img-box">
            <img :src="image" alt="" />
          </div>
          <div class="detail-box">
            <h5>{{ name }}</h5>
            <p>
              Incidunt odit rerum tenetur alias architecto asperiores omnis
              cumque doloribus aperiam numquam! Eligendi corrupti, molestias
              laborum dolores quod nisi vitae voluptate ipsa? In tempore
              voluptate ducimus officia id, aspernatur nihil. Tempore laborum
              nesciunt ut veniam, nemo officia ullam repudiandae repellat
              veritatis unde reiciendis possimus animi autem natus
            </p>
          </div>
        </div>
</template>

<script>
    export default{
        props:["name","image"]
    }
</script>