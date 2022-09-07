<template>
    <div class="container standard_section">
        <h2>{{title}}</h2>
        <div class="card_cont">
            <div class="single_card" v-for="(card, index) in CardData" :key="index">
                <AdvertCard :data="card" />
            </div>
        </div>
    </div>
</template>

<script>
import AdvertCard from './AdvertCard.vue'

export default {
    name:'CoursesAdvertising',
    components:{
        AdvertCard,
    },
    data(){
        return{
            title:'Why my Courses?',
            CardData:[
                {
                    img:'fa-solid fa-briefcase fa-3x',
                    headline:'Entrepreneuership',
                    text:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti itaque nisi eveniet facilis necessitatibus alias suscipit fugit magni dolore laudantium, quis quo ab iusto, similique facere! Molestiae magnam nihil ratione.',
                },
                {
                    img:'fa-solid fa-rocket fa-3x',
                    headline:'Accelerated learning',
                    text:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti itaque nisi eveniet facilis necessitatibus alias suscipit fugit magni dolore laudantium, quis quo ab iusto, similique facere! Molestiae magnam nihil ratione.',
                },
                {
                    img:'fa-regular fa-thumbs-up fa-3x',
                    headline:'Productivity',
                    text:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti itaque nisi eveniet facilis necessitatibus alias suscipit fugit magni dolore laudantium, quis quo ab iusto, similique facere! Molestiae magnam nihil ratione.',
                },
                {
                    img:'fa-solid fa-gear fa-3x',
                    headline:'Life Coaching',
                    text:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deleniti itaque nisi eveniet facilis necessitatibus alias suscipit fugit magni dolore laudantium, quis quo ab iusto, similique facere! Molestiae magnam nihil ratione.',
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
.card_cont{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    padding: 70px 0;
    .single_card{
        width:calc((100% / 2) - 30px);
        margin: 15px;
    }
}   
</style>