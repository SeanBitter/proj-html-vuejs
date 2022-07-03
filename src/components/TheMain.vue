<template>
  <div>
    <MainSection></MainSection>
    <SectionOnlineCourses></SectionOnlineCourses>
    <SmartTutoring></SmartTutoring>
    <MainSectionTwo></MainSectionTwo>
    <StudentsReviews></StudentsReviews>
  </div>
</template>

<script>
import MainSection from './MainSection.vue'
import SectionOnlineCourses from './SectionOnlineCourses.vue'
import SmartTutoring from './SmartTutoring.vue'
import MainSectionTwo from './MainSectionTwo.vue'
import StudentsReviews from './StudentsReviews.vue'

export default {
  components: { MainSection, SectionOnlineCourses, SmartTutoring, MainSectionTwo, StudentsReviews }
}

</script>

<style lang="scss" scoped>

</style>