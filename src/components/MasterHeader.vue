<template>
    <header>
        <HeaderMenuBar/>
        <JumboTron/>
        <IntroductionComp/>
    </header>
</template>

<script>
import HeaderMenuBar from './HeaderMenuBar.vue';
import JumboTron from './JumboTron.vue';
import IntroductionComp from './IntroductionComp.vue';


export default {
    name:'MasterHeader',
    components:{
        HeaderMenuBar,
        JumboTron,
        IntroductionComp,
    }
}
</script>

<style scoped lang="scss">

</style>