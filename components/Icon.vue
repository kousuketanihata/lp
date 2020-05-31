<template>
  <div class="icon">
    <nuxt-link class="detail" to="/test" target="_blank">
      <div class="image-parent">
        <b-img
          class="image"
          thumbnail
          fluid
          rounded="circle"
          :src=image
        ></b-img>
      </div>
      <div class="name">{{ name }}</div>
    </nuxt-link>
  </div>
</template>
<script>
  export default {
    props: ['name','image']
  }
</script>
<style>
  .image {
    width: 100vw;
    vertical-align: middle
  }
  .icon {
    padding: 10px;
    width: 48%;
  }
  .detail {
    text-decoration:none;
    color: #47494e;
  }
  .detail:hover {
    text-decoration:none;
  }
  .name {
    text-align: center;
    font-size: 12px;
    margin-top: 5px;
    margin-bottom: -3px;
  }
  @media screen and (min-width:768px) {
    .icon {
      width: 23%;
    }
    .image {
      /*width: 100vw;*/
      /*height: 17vw;*/
      /*vertical-align: middle*/
    }
  }
</style>
