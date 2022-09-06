<template>
    <div class="container">
        <h2>{{title}}</h2>
        <div class="slider">
            <div>
                <i class="fas fa-arrow-left"></i>
                <div>
                    <img :src="require(imagePath+reviewsList[currentProfile+1].img)" alt="">
                    <img :src="require(imagePath+reviewsList[currentProfile].img)" alt="">
                    <img :src="require(imagePath+reviewsList[currentProfile-1].img)" alt="">
                </div>
                <i class="fas fa-arrow-right"></i>
            </div>
            <div></div>
            <div></div>
        </div>
    </div>
</template>

<script>
export default {
    name:'ReviewsSection',
    data(){
        return{
            currentProfile:1,
            imagePath:'../assets/img/',
            title:'What Students Say',

            reviewsList:[
                {
                    img:'1-100x100.jpg',
                    course:'Shows of the Past',
                    vote:3,
                    text:'Il mio Homer non è comunista. Sarà pure un bugiardo, un maiale, un idiota, un comunista, ma vi assicuro che non è una pornostar.',
                },
                {
                    img:'2-100x100.jpg',
                    course:'Paints of the Future',
                    vote:5,
                    text:'The response to your MasterStudy has been really overwhelming! Those who partecipated in the workshop are spreading the word here on campus and the "buzz" is on. The VP of Instruction wants you to come back! Her goal is to Have more faculty trained. She also wants to attend a workshop herself. Our President told me "MasterStudy needs to be the cornerstone of our success program."',
                },
                {
                    img:'4-100x100.jpg',
                    course:'',
                    vote:4,
                    text:'Mi chiamo Massimo Decimo Meridio, comandante dell’esercito del Nord, generale delle legioni Felix, servo leale dell’unico vero imperatore Marco Aurelio. Padre di un figlio assassinato, marito di una moglie uccisa. E avrò la mia vendetta, in questa vita o nell’altra.',
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">

</style>