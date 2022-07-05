<template>
  <div class="section py-5 mx-auto">
    <div class="container container-newsletter position-relative">

      <h3 class="pb-3">Subscribe <span class="text-my-primary fw-normal">Newsletters</span></h3>
      <p class="text-muted pb-4">Enter your email address to register to our newsletter subscription delivered on a regular basis!</p>

      <form class="d-flex justify-content-center" role="search">
        <input class="form-control bg-light border-0 ps-3 py-2" type="email" placeholder="Enter your email" aria-label="Search">
        <button class="btn-newsletter rounded-end">Subscribe</button>
      </form>

      <div class="overflow-hidden">
        <img :src="require('../assets/img/maxcoach-shape-02.png')" alt="" class="position-img-one">
        <img :src="require('../assets/img/maxcoach-shape-09.png')" alt="" class="position-img-two">
        <span class="position-img-circle"></span>
      </div>

    </div>
  </div>
</template>

<script>
export default {

}

</script>

<style lang="scss" scoped>
@import '../assets/scss/variables';
.container-newsletter {
  margin: auto;
  max-width: 520px;
  width: 100%;
  text-align: center;
  padding: 3rem 0;
}

.btn-newsletter {
  background-color: $primary;
  color: white;
  padding: 1rem 2rem;
  border: 0;
  transition: 0.3s ease-in-out;

    &:hover {
      background-color: $secondary;
    }
}

.position-img-one {
  position: absolute;
  right: -50%;
  bottom: 10%;
  z-index: 1;
}

.position-img-two {
  position: absolute;
  right: -55%;
  top: 3%;
}

.position-img-circle {
  position: absolute;
  bottom: 30%;
  left: -50%;
  border: 8px solid #8FD6CA;
  padding: 1.5rem;
  border-radius: 50%;
}

</style>