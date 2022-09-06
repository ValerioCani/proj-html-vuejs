<template>
    <div class="container">
        <div v-for="(info, index) in businessNumbers" :key="index">
            <!-- <img src="" alt=""> -->
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
                    img:'',
                    quantity:'3195',
                    subject:'Online Learner',
                },
                {
                    img:'',
                    quantity:'23',
                    subject:'Video Courses',
                },
                {
                    img:'',
                    quantity:'437',
                    subject:'Sliders & Images',
                },
                {
                    img:'',
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