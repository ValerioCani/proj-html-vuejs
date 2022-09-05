<template>
    <div class="CourseCard">
        <img :src="require('../assets/img/'+ data.img)" :alt="data.category">
        <div class="datasection">
            <h3>{{data.text}}</h3>
            <h4>{{data.category}}</h4>
            <div class="divider"></div>
            <div>
                <i class="fa-solid fa-signal"></i>{{data.difficulty}}
                <i class="fa-solid fa-list-ul"></i>{{data.lectures}}
                <i class="fa-regular fa-clock"></i>{{data.time}}
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
    .CourseCard{
        width:100%;
        img{
        width: 100%;
        }
        .datasection{
            padding: 20px;
            .divider{
                border: solid grey 1px;
                margin: 10px;
            }
        }
    }
</style>