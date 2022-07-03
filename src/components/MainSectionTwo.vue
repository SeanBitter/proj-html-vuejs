<template>
  <div class="section py-5">
    <div class="container">

      <div class="d-flex flex-row-reverse pb-3">

        <div class="main-section-text my-auto ps-5">
          <h6 class="text-my-tertiary">GET STARTED <span class="border-0 text-my-secondary fw-bold">EFFORTLESSLY</span></h6>
          <h2>Enjoy our <span class="border-0">Companionship</span></h2>
          <p class="pb-3 fs-5">Sneek peek into what has in store for you on our online teaching and mentoring portal. Seek for some hidden hints of early-bird rewards as well.</p>
          <p class="py-3"><span>Download free guidebook<i class="fa-solid fa-arrow-right ps-2"></i></span></p>
        </div>

        <div class="main-section-img my-3 text-start">
          <div class="position-relative">
              <div class="text-center"><img :src="require('../assets/img/home-2-popup-video-poster.jpg')" alt="" class="img-testimonial rounded w-100 shadow"></div>
              <img :src="require('../assets/img/icon-youtube-play.png')" alt="" class="position-img-one-this">
              <img :src="require('../assets/img/maxcoach-shape-05-150x150.png')" alt="" class="position-img-two-this">
              <img :src="require('../assets/img/maxcoach-shape-07-150x150.png')" alt="" class="position-img-three-this">
              <span class="position-img-five-this"></span>
          </div>
        </div>

      </div>

    </div>
  </div>
</template>

<script>

export default {

}

</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";
    .position-img-one-this {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      z-index: 2;
    }

    .position-img-two-this {
      position: absolute;
      top: 10%;
      left: -10%;
      z-index: -1;
    }

    .position-img-three-this {
      position: absolute;
      bottom: -20%;
      right: -2%;
      z-index: -1;
    }

    .position-img-five-this {
      position: absolute;
      top: -10%;
      right: -10%;
      border: 8px solid #ECC5AB;
      padding: 1.5rem;
      border-radius: 50%;
    }

</style>