<template>
  <header>
    <div class="container">
        <img src="@/assets/img/MasterStudy-1.svg" alt="MasterStudy logo">
        <div>
            <ul>
                <li v-for="link in headerMenu" :key="link.index" >
                    <div class="new" v-if="link.new==true">New</div>
                    <h3><a :href="link.url">{{link.text}}</a></h3>
                </li>
            </ul>
            
        </div>
    </div>
  </header>
</template>

<script>
export default {
    name:'MasterHeader',
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
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    header{
        height: 145px;
    }
</style>