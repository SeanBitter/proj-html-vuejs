<template>
  <div class="sticky-top bg-white">
    <div class="container py-3">
      <nav class="nav justify-content-between">

        <div class="d-flex align-items-center">
          <a href="#"><img :src="require('../assets/img/dark-logo.png')" alt="Max Coach" width="150"></a>
        </div>

        <div class="nav">
          <a class="nav-link" href="#" v-for="(link, i) in navbarLinks" :key="i">{{ link }}<i class="fa-solid fa-angle-down"></i></a>
          <a class="my-auto pe-3" href="#"><i class="fa-regular fa-circle-user fs-6"></i></a>
          <form class="d-flex position-relative" role="search">
            <input class="form-control me-2 bg-light border-0 py-2" type="text" placeholder="Search..." aria-label="Search">
            <a href="#"><i class="fa-solid fa-magnifying-glass glass-position fs-6"></i></a>
          </form>
        </div>

      </nav>
    </div>
    <div class="nav-border"></div>
  </div>
</template>

<script>

export default {
  data() {
    return {
      navbarLinks: ["Home", "Pages", "Courses", "Features", "Blog", "Shop"],
    }
  }
}

</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";

  .nav a {
    color: $secondary;
    font-weight: 600;

      i {
        padding-left: 0.5rem;
        font-size: 0.6rem;
      }
  }

  .nav-border {
    // box-shadow: 0px 15px 10px -15px rgb(213, 213, 213);
    // padding: 1rem;
    border-bottom: 4px solid rgba(222, 225, 228, 0.3);
  }

  .glass-position {
    position: absolute;
    top: 50%;
    right: 5%;
    transform: translate(-50%, -50%);
    color: $primary;
  }
</style>