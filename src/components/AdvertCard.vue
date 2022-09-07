<template>
    <div class="card flex">
        <div><i :class="data.img"></i></div>
        <div class="card_text">
            <h3>{{data.headline}}</h3>
            <p>{{data.text}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name:'AdvertCard',
    props:{
        data:Object
    }
}
</script>

<style scoped lang="scss">
@import '@/assets/styles/var.scss';
.card{
    border-left: solid 5px $primary_color;
    padding: 25px;
    box-shadow: 2px 0px 20px 3px rgb(228, 228, 228);
    i{
        color: $primary_color;
        padding:15px;
    }
    .card_text{
        padding:15px;
        h3{
            font-size: 25px;
        }
        p{  
            font-size: 15px;
            line-height: 30px;
            padding: 15px 0;
        }
    }
}
</style>