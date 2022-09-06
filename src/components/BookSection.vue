<template>
    <section>
        <div class="container">
            <div>
                <h2>Get My Exclusive Investing Book just for $19.50</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Repellendus vel aspernatur voluptatem minus obcaecati provident vero perspiciatis nostrum rerum temporibus doloribus.</p>
                <img src="@/assets/img/amazon.png" alt="ordina il libro su amazon">
            </div>
            <div>
                <img src="@/assets/img/book.png" alt="">
            </div>
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
    height: 600px;
    background-image: url('@/assets/img/library.jpg');
    background-position: center;
    .container{
        display: flex;
    }
}

</style>