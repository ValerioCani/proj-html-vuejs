<template>
    <div class="container standard_section">
        <h2>{{title}}</h2>
        <div class="slider_cont">
            <div class="slider flex">
                <i @click="NextReview()" class="fas fa-arrow-left fa-2x"></i>
            
                <img class="profile_image side_image" :src="require('@/assets/img/' + reviewsList[nextProfile].img)" alt="">
                <img class="profile_image central_image" :src="require('@/assets/img/' + reviewsList[currentProfile].img)" alt="">
                <img class="profile_image side_image" :src="require('@/assets/img/' + reviewsList[prevProfile].img)" alt="">
                
                <i @click="PrevReview()" class="fas fa-arrow-right fa-2x"></i>
            </div>
            <div>
                <h3>{{reviewsList[currentProfile].course}}</h3>
                <i v-for="(n, index) in reviewsList[currentProfile].vote" :key="index" class="fas fa-star highlight_text stars"></i>
                <p>{{reviewsList[currentProfile].text}}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'ReviewsSection',
    data(){
        return{
            nextProfile:2,
            currentProfile:1,
            prevProfile:0,
            // imagePath:'@/assets/img/',
            title:'What Students Say',

            reviewsList:[
                {
                    img:'1-100x100.jpg',
                    course:'Design Instruments for Communication',
                    vote:3,
                    text:'Poteva andare meglio',
                },
                {
                    img:'2-100x100.jpg',
                    course:'Paints of the Future',
                    vote:5,
                    text:'The response to your MasterStudy has been really overwhelming! Those who partecipated in the workshop are spreading the word here on campus and the "buzz" is on. The VP of Instruction wants you to come back! Her goal is to Have more faculty trained. She also wants to attend a workshop herself. Our President told me "MasterStudy needs to be the cornerstone of our success program."',
                },
                {
                    img:'4-100x100.jpg',
                    course:'Colossal Italian Dubbing Course',
                    vote:4,
                    text:'Mi chiamo Massimo Decimo Meridio, comandante dell’esercito del Nord, generale delle legioni Felix, servo leale dell’unico vero imperatore Marco Aurelio. Padre di un figlio assassinato, marito di una moglie uccisa. E avrò la mia vendetta, in questa vita o nell’altra.',
                },
                {
                    img:'Abe Simpson.jpg',
                    course:'Shows of the Past',
                    vote:5,
                    text:'Il mio Homer non è comunista. Sarà pure un bugiardo, un maiale, un idiota, un comunista, ma vi assicuro che non è una pornostar.',
                },
            ]
        }
    },
    methods:{
        NextReview(){
            if(this.nextProfile>=this.reviewsList.length-1){
                this.nextProfile=0
            }else{
                this.nextProfile++  
            }
            if(this.currentProfile>=this.reviewsList.length-1){
                this.currentProfile=0
            }else{
                this.currentProfile++  
            }
            if(this.prevProfile>=this.reviewsList.length-1){
                this.prevProfile=0
            }else{
                this.prevProfile++  
            }
        },

        PrevReview(){
            if(this.nextProfile<=0){
                this.nextProfile=this.reviewsList.length-1
            }else{
                this.nextProfile--  
            }
            if(this.currentProfile<=0){
                this.currentProfile=this.reviewsList.length-1
            }else{
                this.currentProfile--  
            }
            if(this.prevProfile<=0){
                this.prevProfile=this.reviewsList.length-1
            }else{
                this.prevProfile--  
            }
        },

    },
}
</script>

<style scoped lang="scss">
.container{
    text-align: center;
    .slider_cont{
        height: 530px;
        max-width: 760px;
        margin: 0 auto;
        .slider{
            justify-content: center;
            align-items: center;
            padding: 40px 0 20px;
            i{
                padding: 0 140px;
            }
            .profile_image{
                border-radius: 50%;
                margin: 8px;
            }
            .side_image{
                height: 70px;
                width: 70px;
            }
            .central_image{
                height: 100px;
                width: 100px;
            }
        }
        h3{
            font-size: 20px;
        }
        .stars{
            margin: 3px;
        }
        p{
            padding: 40px 0;
            line-height: 40px;
            font-size: 18px;
        }
    }
}
</style>