<template>
  <div class="good">
    <div class="card mb-2">
      <b-carousel class="card-img-top" id="carousel-fade" controls fade indicators>
        <b-carousel-slide>
          <template v-slot:img>
            <img class="d-block comic-image" src="~/assets/test/1.jpg" alt="image slot">
          </template>
        </b-carousel-slide>
        <b-carousel-slide>
          <template v-slot:img>
            <img class="d-block comic-image" src="~/assets/test/2.jpg" alt="image slot">
          </template>
        </b-carousel-slide>
      </b-carousel>
      <div class="card-body">
        <b-button
          :href="this.link"
          variant="outline-success"
        >購入ページへ行く
        </b-button>
      </div>
      <div class="card-footer">
        同人誌のタイトルです
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
  .comic-image {
    width: 100%;
    height: 360px;
    object-fit: contain;
    background-color: lightgray;
  }
</style>
