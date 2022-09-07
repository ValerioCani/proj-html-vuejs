<template>
    <div class="CourseCard">
        <div class="img_container flex">
            <div class="special secondary_text" v-if="data.special">SPECIAL</div>
            <img :src="require('../assets/img/'+ data.img)" :alt="data.category">
        </div>

        <div class="datasection">
            <h3>{{data.text}}</h3>
            <h4>{{data.category}}</h4>
            <div class="divider"></div>
            <div class="course_features flex">
                <span><i class="fa-solid fa-signal"></i>{{data.difficulty}}</span>
                <span><i class="fa-solid fa-list-ul"></i>{{data.lectures}} Lectures</span>
                <span><i class="fa-regular fa-clock"></i>{{data.time}}</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'CourseCard',
    props:{
        data:Object,
    }
}
</script>

<style scoped lang="scss">
@import '@/assets/styles/var.scss';
    .CourseCard{
        width:100%;
        position: relative;
        border:solid 1px $card_lines_color;
        .img_container{
            height: 245px;
            overflow: hidden;
            justify-content: center;
            .special{
                position: absolute;
                top: 10px;
                right: 10px;
                font-size: 11px;
                background-color: $special_tag_course_color;
                padding: 1.6% 0.7%;
                border-radius: 3px;
            }
            img{
            height: 100%;
            vertical-align: top;
            }
        }
        .datasection{
            padding: 20px;
            background-color: white;
            text-align: center;
            h3{
                padding: 20px;
            }
            h4{
                padding-bottom: 20px;
                font-weight: 100;
                color: $card_coursecategory_color;
            }
            .divider{
                border-bottom: solid 1px $card_lines_color;
                margin: 10px;
            }
            .course_features{
                justify-content: space-between;
                font-size: 13px;
                i{
                    padding: 5px;
                    font-size: 15px;
                    color: $highlight_text_color;
                }
            }
        }
    }
</style>