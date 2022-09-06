<template>
    <div class="container">
        <div v-for="(info, index) in businessNumbers" :key="index">
            <div>
                <i :class="info.img"></i>
            </div>
            <div>
                <h2>{{info.quantity}}</h2>
                <p>{{info.subject}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'NumbersSection',
    data(){
        return{
            businessNumbers:[
                {
                    img:'fa-solid fa-user-group fa-3x',
                    quantity:'3195',
                    subject:'Online Learner',
                },
                {
                    img:'fa-solid fa-film fa-3x',
                    quantity:'23',
                    subject:'Video Courses',
                },
                {
                    img:'fa-solid fa-photo-film fa-3x',
                    quantity:'437',
                    subject:'Sliders & Images',
                },
                {
                    img:'fa-regular fa-thumbs-up fa-3x',
                    quantity:'1440',
                    subject:'Excellent Reviews',
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">

</style>