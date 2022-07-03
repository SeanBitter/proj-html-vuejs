<template>
  <div class="container end-border">
    <div class="row">
      <div class="col-sm-6 col-md-3" v-for="(statistic, i) in studentsStatistics" :key="i">
        <div class="card-style">
          <h5 class="fw-bold px-5">{{ statistic.title }}</h5>
          <h2 class="text-my-primary fw-bold number-style">{{ statistic.number }}</h2>
          <h6 class="text-my-tertiary fw-bold">{{ statistic.subtitle.toUpperCase()}}</h6>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

  data() {
    return {
      studentsStatistics:[
        {
          title: "Successfully trained",
          number: 1790,
          subtitle: "Enrolled learners",
        },

        {
          title: "Proudly Received",
          number: 19,
          subtitle: "Countrywide awards",
        },
        
        {
          title: "Firmly Established",
          number: 24,
          subtitle: "Local branches",
        },

        {
          title: "Getting Featured on",
          number: 1090,
          subtitle: "Blog posts",
        },
      ],
    }
  }
}

</script>

<style lang="scss" scoped>

.card-style {
  border-left: 2px solid #F8F8F8;
  text-align: center;
  padding: 7rem 0;
}

.number-style {
  font-size: 3rem;
  padding: 1rem 0;
}

.end-border {
  border-right: 2px solid #F8F8F8;
}
</style>