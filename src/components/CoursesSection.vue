<template>
    <section>
        <div class="container">
            <h2>{{title}}</h2>
            <div class="card_cont">
                <div class="single_card" v-for="(card, index) in CardData" :key="index">
                    <CourseCard :data="card"/>
                </div>
                <button>LOAD MORE</button>
            </div>
        </div>       
    </section>
</template>

<script>
import CourseCard from './CourseCard.vue'
export default {
    name:'CoursesSection',
    components:{
        CourseCard,
    },
    data(){
        return{
            title:'New Courses',
            CardData:[
                {
                    img:'ElectronicMusicCourse.jpeg',
                    text:'How to be a DJ? Make Electronic Music',
                    category:'Electronic',
                    difficulty:'Advanced',
                    lectures:8,
                    time:'6 hours',
                },
                {
                    img:'UnrealEngine4.png',
                    text:'Nvidia and UE4 Tecnologies Practice',
                    category:'Nvidia',
                    difficulty:'Advanced',
                    lectures:8,
                    time:'6 hours',
                },
                {
                    img:'FashionPhotographyCourse.jpeg',
                    text:'Fashion Photography from professional',
                    category:'Fashion',
                    difficulty:'Advanced',
                    lectures:6,
                    time:'6 hours',
                },
                {
                    img:'DesignCommunication.jpeg',
                    text:'Design Instruments for Communication',
                    category:'Communication',
                    difficulty:'Intermediate',
                    lectures:6,
                    time:'6 hours',
                },
                {
                    img:'Concept.jpg',
                    text:'Make your Concept Right and Beautiful',
                    category:'Art',
                    difficulty:'Intermediate',
                    lectures:6,
                    time:'6 hours',
                },
                {
                    img:'CyclingCourse.jpeg',
                    text:'Road Bike Manual or How to Be a Champion',
                    category:'Bicycling',
                    difficulty:'Beginner',
                    lectures:6,
                    time:'6 hours',
                },
            ]
           

        }
    }
}

</script>

<style scoped lang="scss">
section{
    background-color: #edf2f5;
    .card_cont{
        width: 100%;
        display: flex;
        flex-wrap: wrap;
        .single_card{
            width:calc((100% / 3) - 20px);
            margin: 10px;
        }
    }
}
</style>