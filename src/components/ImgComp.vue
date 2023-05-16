<script>
    export default {
        name: "ImgComp",
        props: ['propsImg']
    }
</script>

<template>
<div>
    <img :src="propsImg.img" alt="">
</div>
</template>

<style lang="scss" scoped>
    @use '../style/main.scss'as *;

    div {
        width: calc(100% / 4 - 5px);
        img{
            width: 100%;
        }
    }
</style>