<template>
<section>
    <div class="container flex">
        <div class="flex single_stat secondary_text" v-for="(info, index) in businessNumbers" :key="index">
            <div>
                <i :class="info.img"></i>
            </div>
            <div>
                <h3 class="highlight_text">{{info.quantity}}</h3>
                <p>{{info.subject}}</p>
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
    name:'NumbersSection',
    data(){
        return{
            businessNumbers:[
                {
                    img:'fa-solid fa-user-group fa-4x',
                    quantity:'3195',
                    subject:'Online Learner',
                },
                {
                    img:'fa-solid fa-film fa-4x',
                    quantity:'23',
                    subject:'Video Courses',
                },
                {
                    img:'fa-solid fa-photo-film fa-4x',
                    quantity:'437',
                    subject:'Sliders & Images',
                },
                {
                    img:'fa-regular fa-thumbs-up fa-4x',
                    quantity:'1440',
                    subject:'Excellent Reviews',
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
section{
    background-image: url('@/assets/img/counter-1919x1101.jpg');
    background-position-x: center;
    background-size: 112%;
    height: 610px;
    .container{
        height: 100%;
        justify-content: center;
        align-items: center;
        .single_stat{
            padding: 40px;
            i{
                padding-right: 20px;
            }
            h3{
                font-size: 40px;
            }   
        }
    }

}

</style>