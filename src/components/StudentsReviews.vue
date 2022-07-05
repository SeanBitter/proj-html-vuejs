<template>
  <div class="section py-5">

    <h6 class="text-my-tertiary text-center pt-5">GREAT WORDS ABOUT MAXCOACH</h6>
    <h3 class="text-center pb-4">Our <span class="text-my-primary fw-normal">Top Learners'</span> verbatim</h3>

    <div class="row">
      <div class="col-4" v-for="(review, i) in topLearners" :key="i">

        <div class="bg-white rounded p-4 mx-2 h-100">
          <h5 class="py-2">{{ review.title }}</h5>
          <p class="text-my-tertiary pb-3">{{ review.comment }}</p>
          <div class="row">
            <div class="col-3">
              <div class="learners-img">
                <img :src="require('../assets/img/' + review.imgUrl)" :alt="review.name" class="rounded-circle">
              </div>
            </div>
            <div class="col-9 my-auto">
                <h6>{{ review.name.toUpperCase() }}</h6>
                <h6 class="text-my-tertiary">/ {{ review.profession }}</h6>
            </div>
          </div>
        </div>

      </div>
    </div>

    <div class="text-center py-5">
      <span class="dot blue-dot"></span>
      <span class="dot"></span>
      <span class="dot"></span>
      <span class="dot"></span>
    </div>

    <div class="text-center py-4 position-relative">
      <h5>Start today for getting <span class="text-my-primary fw-normal">Online Certification</span></h5>
      <h3>You can be your own guiding star with our help!</h3>
      <div class="pt-4">
        <button class="my-btn">Get started now</button>
      </div>
      <span class="position-img-circle"></span>
      <img :src="require('../assets/img/maxcoach-shape-01.png')" alt="" class="position-img-one">
      <img :src="require('../assets/img/maxcoach-shape-02.png')" alt="" class="position-img-two">
    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      topLearners: [
        {
          title: "It's a choice for quality for people with special needs",
          comment: "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
          imgUrl: "testimonial-avata-03.jpg",
          name: "Florence Themes",
          profession: "Multimedia Admin",
        },

        {
          title: "High level of efficiency and scientific teaching methods",
          comment: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
          imgUrl: "testimonial-avata-02.jpg",
          name: "Mina Hollace",
          profession: "Freelancer",
        },

        {
          title: "Professional team of specialists and passionate mentors at reach",
          comment: "I need to get certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
          imgUrl: "testimonial-avata-04.jpg",
          name: "Madley Pondor",
          profession: "IT Specialist",
        },

        // {
        //   title: "Hello World",
        //   comment: "I am okay.",
        //   imgUrl: "testimonial-avata-01.jpg",
        //   name: "Paolino Paperino",
        //   profession: "Pippo",
        // },
      ],
    }
  }
}

</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";
.section {
  background-color: #F8F8F8;
}

.learners-img {
  max-width: 80px;

    img {
      width: 100%;
    }
}

.dot {
  height: 7px;
  width: 7px;
  border-radius: 50%;
  background-color: $tertiary;
  display: inline-block;
  margin: 0.5rem;
  vertical-align: middle;
}

.blue-dot {
  height: 10px;
  width: 10px;
  background-color: $secondary;
}

.position-img-circle {
  position: absolute;
  top: 15%;
  left: 18%;
  border: 6px solid #E6DCD2;
  padding: 1rem;
  border-radius: 50%;
}

.position-img-one {
  position: absolute;
  top: 40%;
  left: 18%;
}

.position-img-two {
  position: absolute;
  top: 45%;
  right: 18%;
}

</style>