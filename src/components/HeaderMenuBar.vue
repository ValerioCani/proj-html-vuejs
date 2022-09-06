<template>
    <section>
        <div class="container flex">
            <img src="@/assets/img/MasterStudy-1.svg" alt="MasterStudy logo">
            <div class="flex">
                <ul class="flex">
                    <li v-for="link in headerMenu" :key="link.index" >
                        <div class="new" v-if="link.new==true">New</div>
                        <h3><a :href="link.url">{{link.text}}</a></h3>
                        <div class="triangle_up"></div>
                    </li>
                </ul>
                <div class="header_socials" >
                    <a v-for="(social, index) in socialList" :key="index" :href="social.url">
                        <i class="fa-brands" :class="'fa-'+social.social"></i>
                    </a>
                </div>
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
@import '@/assets/styles/var.scss';
    section{
        height: 145px;
        .container{
            height: 100%;
            justify-content: space-between;
            align-items: center;
            ul{
                li{
                    border-bottom: solid 3px transparent;
                    position: relative;
                    margin: 0 15px;
                    h3{
                        margin: 10px 0px;
                    }
                    .new{
                        position:absolute;
                        bottom:32px;
                        right: -14px;
                        font-size: 12px;
                        padding: 1px 3px;
                        border-radius: 3px;
                        color: white;
                        background-color: red;
                    }
                    .triangle_up {
                        width: 0;   
                        height: 0;
                        border-left: 5px solid transparent;
                        border-right: 5px solid transparent;
                        border-bottom: 5px solid transparent;
                        position:absolute;
                        bottom:0px;
                        left: 50%;
                        transform: translate(-50%);
                        
                    }
                    &:hover{
                        border-bottom: solid 3px $primary_color;
                    }
                    &:hover>.triangle_up{
                        border-bottom: 5px solid $primary_color;
                    }
                }
            }

            .header_socials{
                font-size: 20px;
                display: flex;
                align-items: center;
                margin-left: 30px;
                a{
                    margin: 0 8px;
                }  
            }
        }
    }
</style>