<template>
  <section class="footer-section d-flex">
    <!-- LEFT SIDE -->
    <div class="myWrapper d-flex">
      <div class="left-footer-side">
        <div class="container-list">
          <h2 class="text-uppercase footer-links">dc comics</h2>
          <ul class="p-0 mb-0" v-for="(item, index) in DcComics" :key="index">
            <li>{{ item }}</li>
          </ul>
        </div>

        <div class="container-list">
          <h2 class="text-uppercase footer-links">shop</h2>

          <ul class="p-0 mb-0" v-for="(item, index) in Shop" :key="index">
            <li>{{ item }}</li>
          </ul>
        </div>

        <div class="container-list">
          <h2 class="text-uppercase footer-links">dc</h2>

          <ul class="p-0 mb-0" v-for="(item, index) in DCList" :key="index">
            <li>{{ item }}</li>
          </ul>
        </div>

        <div class="container-list">
          <h2 class="text-uppercase footer-links">sites</h2>

          <ul class="p-0 mb-0" v-for="(item, index) in SitesList" :key="index">
            <li>{{ item }}</li>
          </ul>
        </div>
      </div>

      <!-- RIGHT SIDE -->
      <div class="right-footer-side h-100"></div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      DcComics: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],

      Shop: ["Shop Dc", "Shop Dc Collectibles"],

      DCList: [
        "Terms Of Use",
        "Privacy policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],

      SitesList: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
    };
  },
};
</script>

<style lang="scss">
@use '../../../assets/styles/general.scss' as *;

  .footer-section {
    background-image: url(/public/img/footer-bg.jpg);
    background-size: cover;
    height: max-content;
  }

  .left-footer-side {
    width: calc(100% / 2);
    height: 100%;
    display: flex;
  }

  .right-footer-side {
    background-image: url(/public/img/dc-logo-bg.png);
    background-position: center;
    background-repeat: no-repeat;
    z-index: 500;
    color: $hero-img;
    width: calc(100% / 2);
    height: 100%;
  }

  h2 {
    color: white;
  }

  .container-list {
    display: flex;
    flex-flow: column wrap;
    align-items: flex-start;
    padding: 10px;
  }

  .container-list li {
    color: $white;
    list-style: none;
    padding: 5px;
    font-size: 15px;
  }

</style>
