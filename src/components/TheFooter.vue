<template>
  <footer>
    <div class="container">
        <div class="row">

          <div class="col-6">
            <div class="text-my-tertiary">
              <h5 class="text-dark py-3">Address</h5>
              <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
              <p>+1(305)547-9909 (9am - 5pm EST, Monday - Friday)</p>
              <a href="#">support@maxcoach.com</a>
              <div class="fs-4 pt-3 logos">
                <a href="#"><i class="fa-brands fa-facebook-square pe-4"></i></a>
                <a href="#"><i class="fa-brands fa-twitter pe-4"></i></a>
                <a href="#"><i class="fa-brands fa-instagram pe-4"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin pe-4"></i></a>
              </div>
            </div>
          </div>

          <div class="col-6">
            <div class="row">

              <div class="col-3">
                <h5 class="text-dark">Explore</h5>
                <a href="#" v-for="(link, i) in exploreLinks" :key="i">{{ link }}</a>
              </div>

              <div class="col-3">
                <h5 class="text-dark"></h5><br>
                <a href="#" v-for="(link, i) in links" :key="i">{{ link }}</a>
              </div>

              <div class="col-3">
                <h5 class="text-dark">Information</h5>
                <a href="#" v-for="(link, i) in informationLinks" :key="i">{{ link }}</a>
              </div>

            </div>
          </div>

        </div>
        
        <div class="copyright">
          <h6><i class="fa-regular fa-copyright"></i> 2020 MaxCoach. All Rights Reserved</h6>
        </div>

    </div>

    <button class="btn-footer"><i class="fa-solid fa-arrow-up-long"></i></button>

  </footer>
</template>

<script>

export default {
  data() {
    return {
      exploreLinks: ["Start here", "Blog", "About us"],
      links: ["Success story", "Courses", "Contact us",],
      informationLinks: ["Membership", "Purchase guide", "Privacy policy", "Terms of services"],
    }
  }
}

</script>

<style lang="scss" scoped>
@import '../assets/scss/variables';

footer {
  background-color: #F8F8F8;
  padding-top: 4rem;
  padding-bottom: 3rem;
  position: relative;
}

.logos a {
  text-decoration: none;
  color: $tertiary;
  display: inline;
  cursor: pointer;
}

a {
  text-decoration: none;
  color: $tertiary;
  display: block;
  line-height: 32px;
  transition: 0.3s ease-in-out;

    &:hover {
      color: darken($tertiary, 10);
    }
}

.copyright {
  text-align: center;
  color: lighten($tertiary, 10);
  padding-top: 6rem;
}

.btn-footer {
  background-color: $primary;
  color: white;
  height: 65px;
  width: 65px;
  font-size: 1.5rem;
  border-radius: 50%;
  border: 0;
  position: absolute;
  right: 20px;
  bottom: 20px;
  transition: 0.3s ease-in-out;

    &:hover {
      background-color: $secondary;
    }
}
</style>