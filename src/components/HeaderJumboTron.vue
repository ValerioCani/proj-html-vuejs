<template>
    <section>
        <div class="container">
            <div id="title">
                <h1>Start your Human <span class="highlight_text">Revolution</span> today</h1>
                <p>A wonderful serenity has taken possessionof my entire soul, like these sweet mornings of spring which I enjoy with my whole heart.</p>
            </div>
            <div id="course_sale" class="flex">
                <div>
                    <h2><span class="secondary_text">Limited Sale:</span> All courses with 55% off</h2>
                    <input type="email">
                    <button>SUBSCRIBE</button>
                </div>
                <div class="flex">
                    <div class="time">
                        <div class="num">26</div>
                        <div class="unit">Days</div>
                    </div>
                    <div class="time">
                        <div class="num">01</div>
                        <div class="unit">Hours</div>
                    </div>
                    <div class="time">
                        <div class="num">47</div>
                        <div class="unit">Minutes</div>
                    </div>
                    <div class="time">
                        <div class="num">34</div>
                        <div class="unit">Seconds</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:'JumboTron',
}
</script>

<style scoped lang="scss">
@import '@/assets/styles/var.scss';
    section{
        height: 835px;
        background-image: url('../assets/img/slide-1.jpg');
        background-position: center;
        .container{
            height: 100%;
            position: relative;
            #title{
                width: 600px;
                position: relative;
                top: 210px;
                left: 510px;
                h1{
                    font-size: 70px;
                    margin-bottom: 30px;
                }
                p{
                    line-height: 30px;
                    font-size: 18px;
                }
            }
            #course_sale{
                width: 1310px;
                height: 242px;
                background-color: $primary_color;
                border-radius: 10px;
                position: absolute;
                top: 670px;
                justify-content: center;
                align-items: center;
                h2{
                    font-size: 30px;
                }
                .time{
                
                }
            }
        }
    }
</style>