<template>
    <main>
        <CoursesSection/>
        <BookSection/>
    </main>
</template>

<script>
import CoursesSection from './CoursesSection.vue'
import BookSection from './BookSection.vue'

export default {
    name:'MasterMain',
    components: {
        CoursesSection,
        BookSection,
    },
}
</script>

<style scoped lang="scss">

</style>