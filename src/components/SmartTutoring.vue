<template>
  <div class="section py-5">
    <div class="container">

      <h6 class="text-my-tertiary text-center pt-5 fw-normal">MAX COACH AVAILABLE COURSES</h6>
      <h3 class="text-center">Access <span class="text-my-primary fw-normal">Smart Tutoring</span> Program for Benefits.</h3>

      <div class="row">
        <div class="col-4" v-for="(tutoring, i) in smartTutoring" :key="i">
          <div class="py-5 px-4">
            <div>
              <img :src="require('../assets/img/' + tutoring.imgUrl)" :alt="tutoring.title">
            </div>
            <h5 class="pt-4 pb-2">{{ tutoring.title }}</h5>
            <p class="text-my-tertiary fw-normal lh-base">{{ tutoring.description }}</p>
            <a class="text-my-tertiary fw-bold">{{ tutoring.link }} <i class="fa-solid fa-arrow-right"></i></a>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      smartTutoring: [
        {
          imgUrl: "home-2-image-box-01.png",
          title: "Customize preferences",
          description: "Learners are given the right to arrange and customize their study schedule and timetable based on preferences.",
          link: "Start here"
        },

        {
          imgUrl: "about-us-02-image-box-02.png",
          title: "Cloud Storage",
          description: "You can store online lessons via online cloud or download to your device and revise lessons on the way.",
          link: "Get Free Quote"
        },

        {
          imgUrl: "home-2-image-box-03.png",
          title: "Multimedia Channels",
          description: "We provide study materials with various formats: video, audio, slides, doc, prints, books and applications.",
          link: "Start now"
        },
      ],
    }
  }
}
</script>

<style lang="scss" scoped>

</style>