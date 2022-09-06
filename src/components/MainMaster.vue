<template>
    <main>
        <MainCoursesSection/>
        <MainBookSection/>
        <MainCoursesAdvertising/>
        <MainNumbersSection/>
        <MainReviewsSection/>
    </main>
</template>

<script>
import MainCoursesSection from './MainCoursesSection.vue'
import MainBookSection from './MainBookSection.vue'
import MainCoursesAdvertising from './MainCoursesAdvertising.vue'
import MainNumbersSection from './MainNumbersSection.vue'
import MainReviewsSection from './MainReviewsSection.vue'



export default {
    name:'MasterMain',
    components: {
        MainCoursesSection,
        MainBookSection,
        MainCoursesAdvertising,
        MainNumbersSection,
        MainReviewsSection,
    },
}
</script>

<style scoped lang="scss">

</style>