<template>
  <div class="section py-5">
    <div class="container">

      <h6 class="text-my-tertiary text-center fw-normal">SIMULATED TO LEARN?</h6>
      <h3 class="text-center">Featured Online Courses</h3>

      <div class="row">
        <div class="col-6 py-5" v-for="(course, i) in onlineCoursesDetails" :key="i">
          <div class="row">
            <div class="col-4">
              <div>
                <img :src="require('../assets/img/' + course.imgUrl)" :alt="course.title" class="rounded-circle rario ratio-1x1 w-100">
              </div>
            </div>
            <div class="col-8">
              <h4 class="text-my-primary">{{ course.price}}</h4>
              <h5>{{ course.title }}</h5>
              <p class="text-my-tertiary"><i class="fa-regular fa-file-lines pe-2"></i> {{ course.lessons }} Lessons <span class="ps-4"><i class="fa-solid fa-user-large pe-2"></i> {{ course.students }} Students</span></p>
            </div>
          </div>
        </div>
      </div>

      <div class="text-center pb-5">
        <button class="my-btn">View all courses <i class="fa-solid fa-arrow-right"></i> </button>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      onlineCoursesDetails: [
        {
          imgUrl: "course-02-480x298.jpg",
          price: "$40.00",
          title: "Learning to Write as a Professional Author",
          lessons: 20,
          students: 50,
        },

        {
          imgUrl: "stock-full-hd-03-480x298.jpg",
          price: "Free",
          title: "Customic-centric Info-tech Strategies",
          lessons: 24,
          students: 769,
        },

        {
          imgUrl: "stock-full-hd-04-480x298.jpg",
          price: "$19.00",
          title: "Open Programming Courses for Everyone: Python",
          lessons: 17,
          students: 62,
        },

        {
          imgUrl: "stock-full-hd-06-480x298.jpg",
          price: "$26.00",
          title: "Academic Listening and Note-taking",
          lessons: 14,
          students: 67,
        },

        {
          imgUrl: "course-featured-image-01-480x298.jpg",
          price: "$39.00",
          title: "Master jQuery in a Short Period of Time",
          lessons: 6,
          students: 51,
        },

        {
          imgUrl: "stock-full-hd-05-480x298.jpg",
          price: "$59.00",
          title: "Introduction to Javascript for Beginners",
          lessons: 14,
          students: 76,
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";

.section {
  background-color: #F5F7FA;
}

h3, h4, h5 {
  font-weight: 600;
  line-height: 32px;
  transition: 0.3s ease-in-out;
}

h5:hover {
  color: $primary;
  cursor: pointer;
}

img {
  aspect-ratio: 1;
  max-width: 100%;
  object-fit: cover;
}

</style>