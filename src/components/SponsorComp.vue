<script>
    export default {
        name: "SponsorComp",
    }
</script>

<template>
    <div class="text-center">
        <h4>SPONSOR</h4>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis temporibus, quis aut architecto</p>
    </div>

    <div class="sponsor w-75 mx-auto my-5 d-flex justify-content-between">
        <img src="/images/banner-1.jpg" alt="">
        <img src="/images/banner-2.jpg" alt="">
        <img src="/images/banner-3.jpg" alt="">
        <img src="/images/banner-4.jpg" alt="">
        <img src="/images/banner-5.jpg" alt="">
        <img src="/images/banner-6.jpg" alt="">
    </div>
</template>

<style lang="scss" scoped>
    @use '../style/main.scss'as *;
div{
    padding-top: 40px;
    width: 300px;
    margin: 0 auto;
    h4 {
        font-size: 30px;
    }

    p {
        font-size: 14px;
        color: $Natural-Gray;
    }
}
</style>