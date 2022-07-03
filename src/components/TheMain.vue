<template>
  <div>
    <MainSection></MainSection>
    <SectionOnlineCourses></SectionOnlineCourses>
    <SmartTutoring></SmartTutoring>
    <MainSectionTwo></MainSectionTwo>
  </div>
</template>

<script>
import MainSection from './MainSection.vue'
import SectionOnlineCourses from './SectionOnlineCourses.vue'
import SmartTutoring from './SmartTutoring.vue'
import MainSectionTwo from './MainSectionTwo.vue'

export default {
  components: { MainSection, SectionOnlineCourses, SmartTutoring, MainSectionTwo }
}

</script>

<style lang="scss" scoped>

</style>