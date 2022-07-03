<template>
  <div class="section py-5">
    <div class="container">

      <div class="d-flex pb-3">

        <div class="main-section-text my-auto">
          <h2>Distant learning for further expansion</h2>
          <p class="pb-3 fs-5">Learning is a life-long-journey that in fact we never find the terminate stop. Stop searching, enjoy the process.</p>
          <button class="my-btn my-3"><i class="fa-solid fa-download pe-3"></i>Download free guide</button>
          <p class="py-3">Have questions? <span>Get Free Sample<i class="fa-solid fa-arrow-right ps-2"></i></span></p>
        </div>

        <div class="main-section-img my-3 text-end">
          <div class="position-relative">
            <div class="text-end"><img :src="require('../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg')" alt="" class="rounded-circle img-testimonial ms-5"></div>
            <img :src="require('../assets/img/maxcoach-shape-08.png')" alt="" class="position-img-one">
            <img :src="require('../assets/img/maxcoach-shape-08.png')" alt="" class="position-img-two">
            <img :src="require('../assets/img/maxcoach-shape-07-150x150.png')" alt="" class="position-img-three">
            <img :src="require('../assets/img/maxcoach-shape-02.png')" alt="" class="position-img-four">
            <span class="position-img-circle"></span>
          </div>
        </div>

      </div>

      <div class="row py-3">
        <div class="col-sm-6 col-md-4 col-lg-2 d-flex align-items-center justify-content-center py-3" v-for="logo in logos" :key="logo.name">
          <img :src="logosUrl(logo.imgCode)" :alt="logo.name" class="opacity-50">
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'MainSection',

  data() {
    return {
      logos: [
        {
          name: "stylus",
          imgCode: "01",
        },

        {
          name: "tree",
          imgCode: "02",
        },

        {
          name: "brook",
          imgCode: "03",
        },

        {
          name: "pencil",
          imgCode: "04",
        },

        {
          name: "it's alive",
          imgCode: "05",
        },

        {
          name: "six base",
          imgCode: "06",
        },

      ],
    }

  },

    methods: {
      logosUrl(code) {
        return require("../assets/img/client-logo-" + code + ".png");
      }
    }
}

</script>

<style lang="scss">
@import "../assets/scss/variables";

  .main-section-text {
    flex-basis: 45%;

      h2 {
        font-size: 2.5rem;
        font-weight: 600;
      };

      p {
        color: $tertiary;
      }

      span {
        color: $primary;
        border-bottom: 1px solid lighten($tertiary, 20%);
      }
  }

  .main-section-img {
    flex-basis: 55%;

      .img-testimonial {
        max-width: 100%;
      }
      .position-img-one {
        position: absolute;
        top: 30%;
        left: 5%;
        z-index: -1;
      }

      .position-img-two {
        position: absolute;
        top: 54%;
        left: 5%;
        z-index: -1;
      }

      .position-img-three {
        position: absolute;
        bottom: 5%;
        right: 80px;
        z-index: -1;
      }

      .position-img-four {
        position: absolute;
        bottom: 60%;
        right: -15%;
      }

      .position-img-circle {
        position: absolute;
        bottom: 22%;
        left: 10%;
        border: 8px solid #ECC5AB;
        padding: 1.5rem;
        border-radius: 50%;
      }
  }
</style>