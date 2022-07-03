<template>
  <div>
    <MainSection></MainSection>
    <SectionOnlineCourses></SectionOnlineCourses>
    <SmartTutoring></SmartTutoring>
    <MainSectionTwo></MainSectionTwo>
    <StudentsReviews></StudentsReviews>
    <StatisticsSection></StatisticsSection>
  </div>
</template>

<script>
import MainSection from './MainSection.vue'
import SectionOnlineCourses from './SectionOnlineCourses.vue'
import SmartTutoring from './SmartTutoring.vue'
import MainSectionTwo from './MainSectionTwo.vue'
import StudentsReviews from './StudentsReviews.vue'
import StatisticsSection from './StatisticsSection.vue'

export default {
  components: { MainSection, SectionOnlineCourses, SmartTutoring, MainSectionTwo, StudentsReviews, StatisticsSection }
}

</script>

<style lang="scss" scoped>

</style>