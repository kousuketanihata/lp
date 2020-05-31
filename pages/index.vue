<template>
 <div class="parent">
   <Header/>
    <div class="container">
      <div class="description">
        説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ
        説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ説明分が入るよ
        掲載依頼は<a href="xxxxx">こちら</a>からお願い致します
      </div>
      <div class="flex">
        <Icon name="Hello フック!" image="/images/icon/kai.jpg"></Icon>
        <Icon name="Hello ピーター!" image="https://picsum.photos/250/250/?image=54"></Icon>
        <Icon name="Hello デス・フック!" image="https://picsum.photos/250/250/?image=58"></Icon>
        <Icon name="Hello フック!" image="https://picsum.photos/250/250/?image=59"></Icon>
        <Icon name="Hello ピーター!" image="https://picsum.photos/250/250/?image=54"></Icon>
        <Icon name="Hello デス・フック!" image="https://picsum.photos/250/250/?image=58"></Icon>
        <Icon name="Hello フック!" image="https://picsum.photos/250/250/?image=54"></Icon>
        <Icon name="Hello ピーター!" image="https://picsum.photos/250/250/?image=58"></Icon>
        <Icon name="Hello デス・フック!" image="https://picsum.photos/250/250/?image=59"></Icon>
      </div>
    </div>
   <Footer/>
  </div>
</template>
<script>
  import Header from '~/components/Header.vue'
  import Icon from "../components/Icon.vue";
  import Footer from '~/components/Footer.vue'

  export default {
    components: {
      Icon,
      Header,
      Footer
    }
  }
</script>
<style scoped>
  @media screen and (min-width:768px) {
    .description {
      margin: 12px;
    }
  }
  .description {
    border: 1px solid rgba(0, 0, 0, 0.125);
    border-radius: 0.25rem;
    margin: 5px;
    margin-top: 9px;
    font-size: 11px;
    padding: 4px;
    background-color: #FFFFFF;
  }
  .icon {
    border: 1px solid rgba(0, 0, 0, 0.125);
    border-radius: 0.25rem;
    margin: 1%;
  }
  .flex {
    background-color: #FFFFFF;
    display: flex;
    flex-wrap: wrap;
    padding: 1px;
  }
  .parent {
    background-color: #F3F5F8;
  }
</style>
