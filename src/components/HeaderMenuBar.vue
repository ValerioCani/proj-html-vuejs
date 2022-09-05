<template>
    <section>
        <div class="container">
            <img src="@/assets/img/MasterStudy-1.svg" alt="MasterStudy logo">
            <div>
                <ul>
                    <li v-for="link in headerMenu" :key="link.index" >
                        <div class="new" v-if="link.new==true">New</div>
                        <h3><a :href="link.url">{{link.text}}</a></h3>
                    </li>
                </ul>
                <a v-for="(social, index) in socialList" :key="index" :href="social.url">
                    <i class="fa-brands" :class="'fa-'+social.social"></i>
                </a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'HeaderMenuBar',
    data(){
        return{
            headerMenu:[
                {
                    text:'Courses',
                    url:'#',
                    index: 1,
                    new: false
                },
                {
                    text:'Course Formats',
                    url:'#',
                    index: 2,
                    new: false
                },
                {
                    text:'Add Course',
                    url:'#',
                    index: 3,
                    new: true
                },
                {
                    text:'Pages',
                    url:'#',
                    index: 4,
                    new: false
                },
                {
                    text:'Demos',
                    url:'#',
                    index: 5,
                    new: false
                },
            ],

            socialList:[
                {
                    social:'linkedin',
                    url:'#',
                },
                {
                    social:'instagram',
                    url:'#',
                },
                {
                    social:'facebook',
                    url:'#',
                },
                {
                    social:'twitter',
                    url:'#',
                },
            ],
        }
    }
}
</script>

<style scoped lang="scss">
    section{
        height: 145px;
    }
</style>