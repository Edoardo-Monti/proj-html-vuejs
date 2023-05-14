<script>
    export default {
        name: "SpeakerComp",
    }
</script>

<template>
    <div class="box">
        <div class="title w-75 mx-auto d-flex justify-content-between">
            <h3>SPEAKERS</h3>

        </div>
        <div id="carouselExampleIndicators" class="carousel slide w-75 mx-auto">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active"
                    aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"
                    aria-label="Slide 2"></button>
            </div>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <div class="d-flex justify-content-between">
                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-6.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Patrick Spencer</h5>
                                <p class="card-text">S&P Analyzer</p>
                            </div>
                        </div>

                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-5.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Janet Jones</h5>
                                <p class="card-text">Newyork Post's GM</p>
                            </div>
                        </div>

                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-4.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Michael Dover</h5>
                                <p class="card-text">Starbuck's CEO</p>
                            </div>
                        </div>

                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-3.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Angelina Holy</h5>
                                <p class="card-text">Maxi's Manager</p>
                            </div>
                        </div>
                        
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="d-flex justify-content-between">
                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-2.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Patrick Spencer</h5>
                                <p class="card-text">S&P Analyzer</p>
                            </div>
                        </div>

                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-1.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Jone Jones</h5>
                                <p class="card-text">Newyork Post's GM</p>
                            </div>
                        </div>

                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-7.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Michael Dover</h5>
                                <p class="card-text">Starbuck's CEO</p>
                            </div>
                        </div>

                        <div class="card" style="width: 18rem;">
                            <img src="/images/speaker-8.jpg" class="card-img-top" alt="...">
                            <div class="card-body text-center">
                                <h5 class="card-title">Angelina Holy</h5>
                                <p class="card-text">Maxi's Manager</p>
                            </div>
                        </div>
                        
                    </div>
                </div>
            </div>

        </div>


    </div>

</template>

<style lang="scss" scoped>
    @use '../style/main.scss'as *;

    .box {
        padding: 70px 0;
        background-color: $Cloud;
        div{
            h3{
                padding-bottom: 50px;
            }
        }
        .card{
            border: none;
            .card-body{
                background-color: $Cloud;
                border: none;
            }
        }
    }
</style>