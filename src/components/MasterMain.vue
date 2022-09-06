<template>
    <main>
        <CoursesSection/>
        <BookSection/>
        <CoursesAdvertising/>
        <NumbersSection/>
        <ReviewsSection/>
    </main>
</template>

<script>
import CoursesSection from './CoursesSection.vue'
import BookSection from './BookSection.vue'
import CoursesAdvertising from './CoursesAdvertising.vue'
import NumbersSection from './NumbersSection.vue'
import ReviewsSection from './ReviewsSection.vue'



export default {
    name:'MasterMain',
    components: {
        CoursesSection,
        BookSection,
        CoursesAdvertising,
        NumbersSection,
        ReviewsSection,
    },
}
</script>

<style scoped lang="scss">

</style>