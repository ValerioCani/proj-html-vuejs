<template>
    <section>
        <div class="container flex">
            <div id="book_ads">
                <h2 class="highlight_text">Get My Exclusive Investing Book just for $19.50</h2>
                <p class="secondary_text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Repellendus vel aspernatur voluptatem minus obcaecati provident vero perspiciatis.</p>
                <img src="@/assets/img/amazon.png" alt="ordina il libro su amazon">
            </div>
            <img src="@/assets/img/book.png" alt="ordina il libro su amazon">
        </div>
    </section>
</template>

<script>
export default {
    name:'BookSection',
}
</script>

<style scoped lang="scss">
section{
    background-image: url('@/assets/img/library.jpg');
    background-position: center;
    height: 600px;
    .container{
        height: 100%;
        padding-top: 50px;
        #book_ads{
            width: 50%;
            height: 100%;
            text-align: center;
            h2{
                font-size: 40px;
                padding-top: 70px;
            }
            p{
            font-size: 25px;
            font-style: italic;
            line-height: 40px;
            padding: 40px 0;
            }
        }
    }
}

</style>