<template>
    <div class="card">
        <!-- <img :src="require('@/assets/img/'+ data.img)" :alt="data.headline"> -->
        <div>
            <h2>{{data.headline}}</h2>
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
.card{
    border-left: solid 5px #f2b91e;
}
</style>