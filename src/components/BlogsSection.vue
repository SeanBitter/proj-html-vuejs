<template>
  <div class="section">
    <div class="container py-5">

      <div class="row">

        <div class="col-sm-12 col-md-4">
          <div class="pt-5">
            <h6 class="text-my-tertiary">ENJOYABLE INSIGHTS</h6>
            <h3 class="fw-bold py-3">Most Viewed <span class="text-my-primary fw-normal">Best Blogs</span></h3>
            <ul class="list-unstyled">
              <li class="py-3 fw-bold" v-for="(blogList, i) in blogsList" :key="i"><i class="fa-solid fa-right-long pe-3"></i>{{ blogList }}</li>
            </ul>
          </div>
        </div>

        <div class="col-sm-12 col-md-4" v-for="(blog, i) in bestBlogs" :key="i">
          <div class="shadow m-3 rounded bg-white">
            <div>
              <img :src="require('../assets/img/' + blog.imgUrl)" :alt="blog.title" class="w-100 rounded-top">
            </div>

            <div class="p-4">
              <h6 class="text-my-tertiary fw-bold">{{ blog.profession.toUpperCase()}}</h6>
              <h5 class="fw-bold lh-base py-3">{{ blog.title }}</h5>
              <h6 class="text-my-tertiary"><i class="fa-regular fa-calendar pe-2"></i> {{ blog.date }} <span class="ps-4"><i class="fa-regular fa-eye pe-2"></i> {{ blog.views }} views</span></h6>
            </div>

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
      blogsList: [
        "Become a Better Blogger: Content Planning",
        "Promoting your Online Business on Pinterest",
        "Gamification and Game-Based Learning",
        "Designing an Online Course from Expert's Perspective",
        "Why Online Courses Are the Future of Education",
      ],

      bestBlogs: [
        {
          imgUrl: "artist-blog-03-480x352.jpeg",
          profession: "Artist",
          title: "Brush Strokes Energize Trees in Paintings",
          date: "May 15, 2020",
          views: 688,
        },

        {
          imgUrl: "artist-blog-01-480x352.jpg",
          profession: "Artist",
          title: "Pocket-Sized Notebooks Hold Miniature Paintings",
          date: "May 15, 2020",
          views: 603,
        },
      ],
    }
  }
}

</script>

<style lang="scss" scoped>
.section {
  background-color: #F5F1ED;
  padding: 5rem 0;
}

</style>