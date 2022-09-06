<template>
    <header>
        <HeaderMenuBar/>
        <HeaderJumboTron/>
        <HeaderIntroductionComp/>
    </header>
</template>

<script>
import HeaderMenuBar from './HeaderMenuBar.vue';
import HeaderJumboTron from './HeaderJumboTron.vue';
import HeaderIntroductionComp from './HeaderIntroductionComp.vue';


export default {
    name:'MasterHeader',
    components:{
        HeaderMenuBar,
        HeaderJumboTron,
        HeaderIntroductionComp,
    }
}
</script>

<style scoped lang="scss">

</style>