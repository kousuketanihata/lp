<template>
  <div class="inner">
    <Header/>
    <div class="container">
      <div class="user">
        <Icon
          name="Hello フック!"
          image="/images/icon/kai.jpg"
        ></Icon>
        <div class="profile">
          <h2 class="pc-name">
            Hello フック!
          </h2>
          まわりはひものかっこう沢山者をおかげをのきゴーシュたた。
          するとすこし楽たますってかっこうないた。
          下手ましたのうはたするとゴーシュの勝手らのままにはばた
        </div>
      </div>
      <div class="goods">
        <Comic
          link="https://booth.pm/ja/items/905306"
        />
        <Good
          content="アクキーAです"
          link="https://booth.pm/ja/items/905306"
          image="/images/test/good_d.png"
        />
        <Good
          content="アクキーBです"
          link="https://booth.pm/ja/items/905306"
          image="/images/test/good_b.png"
        />
      </div>
    </div>
    <Footer/>
  </div>
</template>
<script>
  import Header from '~/components/Header.vue'
  import Icon from "../components/Icon";
  import Comic from '~/components/items/Comic.vue';
  import Good from '~/components/items/Good.vue';
  import Footer from '~/components/Footer.vue'

  export default {
    components: {
      Icon,
      Header,
      Comic,
      Good,
      Footer
    }
  }
</script>
<style scoped>
  .user {
    margin-top: 10px;
    width: 100%;
    border: 1px solid rgba(0, 0, 0, 0.125);
    background-color: #FFFFFF;
    border-radius: 0.25rem;
    display: flex;
  }
  .icon {
    /*margin: 0 auto;*/
  }
  .profile {
    width: 50%;
    font-size: 13px;
    margin-top: 10px;
  }
  .inner {
    background-color: #F3F5F8;
  }
  .pc-name {
    display: none;
  }
  @media screen and (min-width:768px) {
    .goods {
      display: flex;
    }
    .good {
      max-width: 33%;
      margin-right: 1%;
    }
    .pc-name {
      display: block;
      font-size: 15px;
      line-height: 18px;
    }

    >>> .name {
      display: none;
    }
  }
</style>
