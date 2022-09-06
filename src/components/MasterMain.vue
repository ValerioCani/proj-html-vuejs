<template>
    <main>
        <CoursesSection/>
        <BookSection/>
        <CoursesAdvertising/>
    </main>
</template>

<script>
import CoursesSection from './CoursesSection.vue'
import BookSection from './BookSection.vue'
import CoursesAdvertising from './CoursesAdvertising.vue'

export default {
    name:'MasterMain',
    components: {
        CoursesSection,
        BookSection,
        CoursesAdvertising,
    },
}
</script>

<style scoped lang="scss">

</style>