<template>
  <div class="section py-5">
    <div class="container">

      <div class="d-flex flex-row-reverse pb-3">

        <div class="main-section-text my-auto">
          <h6>GET STARTED <span>EFFORTLESSLY</span></h6>
          <h2>Enjoy our <span>Companionship</span></h2>
          <p class="pb-3 fs-5">Sneek peek into what has in store for you on our online teaching and mentoring portal. Seek for some hidden hints of early-bird rewards as well.</p>
          <p class="py-3"><span>Download free guidebook<i class="fa-solid fa-arrow-right ps-2"></i></span></p>
        </div>

        <!-- sistemare le img in absolute, aggiungere logo yt, sistemare colori titolo  -->

        <div class="main-section-img my-3 position-relative text-start">
          <img :src="require('../assets/img/home-2-popup-video-poster.jpg')" alt="" class="img-testimonial rounded">
          <img :src="require('../assets/img/maxcoach-shape-08.png')" alt="" class="position-img-one">
          <img :src="require('../assets/img/maxcoach-shape-08.png')" alt="" class="position-img-two">
          <img :src="require('../assets/img/maxcoach-shape-07-150x150.png')" alt="" class="position-img-three">
          <img :src="require('../assets/img/maxcoach-shape-02.png')" alt="" class="position-img-four">
          <span class="position-img-five"></span>
        </div>

      </div>

    </div>
  </div>
</template>

<script>

export default {

}

</script>

<style lang="scss">
@import "../assets/scss/variables";

</style>