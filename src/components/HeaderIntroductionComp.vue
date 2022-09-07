<template>
    <div class="container flex">
        <div class="intro_column1">
            <h2>Hey there, my name is Jhon Doe. I'm the founder of the Brain Academy.</h2>
            <img src="../assets/img/sign.jpg" alt="">
            <div class="clear"></div>
        </div>
        <div class="intro_column2">
            <p>A wonderful serenity has taken possessionof my entire soul, like these sweet mornings of spring which I enjoy with my whole heart. I am alone, and feel the charm of existence in this spot, which was created for the bliss do souls like mine. I am so happy, my dear friend, so absorbed in the exquisite sense of mere tranquil existence, that I neglect my tslents. When, while the lovely valley teems with vapour around me, and the meridian sun stikes the upper surface of the impenetrable foliage of my trees, and but a few stray gleams steal into the inner sanctuary</p>
        </div>
    </div>
</template>

<script>
export default {
    name:'IntroductionComp',
}
</script>

<style scoped lang="scss">
.container{
    padding: 200px 0 100px 0;
    .intro_column1{
        width: 40%;
        h2{
            font-size: 38px;
        }
        img{
        float: right;
        padding-top: 50px;
        }
    }
    .intro_column2{
        width: 60%;
        padding-left: 70px;
        h2{
            font-size: 40px;
        }
    }
    
    p{
            line-height: 35px;
        }
}

</style>