<template>
    <header>
        <HeaderMenuBar/>
        <JumboTron/>
    </header>
</template>

<script>
import HeaderMenuBar from './HeaderMenuBar.vue';
import JumboTron from './JumboTron.vue';

export default {
    name:'MasterHeader',
    components:{
        HeaderMenuBar,
        JumboTron
    }
}
</script>

<style scoped lang="scss">

</style>