<template>
  <div>
    <MainSection></MainSection>
    <OnlineCourses></OnlineCourses>
    <SmartTutoring></SmartTutoring>
    <MainSectionTwo></MainSectionTwo>
    <StudentsReviews></StudentsReviews>
    <StatisticsSection></StatisticsSection>
    <BlogsSection></BlogsSection>
    <TheNewsletter></TheNewsletter>
  </div>
</template>

<script>
import MainSection from './MainSection.vue'
import OnlineCourses from './OnlineCourses.vue'
import SmartTutoring from './SmartTutoring.vue'
import MainSectionTwo from './MainSectionTwo.vue'
import StudentsReviews from './StudentsReviews.vue'
import StatisticsSection from './StatisticsSection.vue'
import BlogsSection from './BlogsSection.vue'
import TheNewsletter from './TheNewsletter.vue'

export default {
  components: { MainSection, OnlineCourses, SmartTutoring, MainSectionTwo, StudentsReviews, StatisticsSection, BlogsSection, TheNewsletter, }
}

</script>

<style lang="scss" scoped>

</style>