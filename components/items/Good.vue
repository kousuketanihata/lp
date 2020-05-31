<template>
  <div class="good">
    <div class="card mb-2">
      <img
        :src="this.image"
        alt="Image"
        class="card-img-top trim">
      <div class="card-body">
        <b-button
        :href="this.link"
        target="_blank"
        variant="outline-success"
      >購入ページへ行く
      </b-button>
      </div>
      <div class="card-footer">
        {{ content }}
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    props: ['link','image','content']
  }
</script>
<style>
  .good {
    margin-top: 10px;
    margin-bottom: 10px;
  }
  .trim {
    overflow: hidden;
    object-fit: scale-down;
    max-height: 365px;
    position: relative;
    background-color: lightblue;
  }
</style>
