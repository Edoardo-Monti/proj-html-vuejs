<script>
    import VideoComp from './VideoComp.vue';

    export default {
        name: "Presentation",
        components: {
            VideoComp
        }
    }
</script>

<template>
    <div class="box w-75 mx-auto d-flex justify-content-between">
        <div>
            <h4>PRESENTATION</h4>
            <VideoComp />
        </div>
        <div class="twit">
            <h4>TWITTER FEED</h4>
            <div class="d-flex">
                <i class="fa-brands fa-twitter" style="color: #97dff7;"></i>
                <p>Stand out and be vibrant with some of the best bright and bold templates on <a href="">@Envato</a>
                    Elements. And add splash of <a href="">https://t.co/vvsdsvs</a></p>
            </div>
            <div class="d-flex">
                <i class="fa-brands fa-twitter" style="color: #97dff7;"></i>
                <p>Do you need to deliver the perfect presentation or creative pitch? Sure, your ideas and plans need to
                    be on-point <a href="">https://t.co/vvsdsvs</a></p>
            </div>
            <div class="d-flex">
                <i class="fa-brands fa-twitter" style="color: #97dff7;"></i>
                <p>Cut yourself a piece of the BFCM sales pie with a solid marketing plan. Here are 5 ways to ptimaze
                    ypur content <a href="">https://t.co/vvsdsvs</a></p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../style/main.scss'as *;

    .box {
        padding: 30px 0;
        h4{
            margin-bottom: 40px;
        }

        .twit {
            margin-left: 50px;
            div {
                margin: 50px 0;
                a {
                    color: $Scarlet;
                    text-decoration: none;
                    font-style: italic;
                }
                i{
                    margin-right: 25px;
                    font-size: 30px;
                }

                p {
                    font-size: 14px;
                    color: $Natural-Gray;
                }
            }
        }
    }
</style>