<script>
    export default {
        name: "NewsComp",
    }
</script>

<template>
    <div class="box">
        <div class="title w-75 mx-auto d-flex justify-content-between align-items-center">
            <div class="inline">
                <h3>RECENT NEWS</h3>
            </div>
            <a href="">Read All News</a>
        </div>

        <div class="w-75 mx-auto d-flex justify-content-between align-items-center">
            <div class="card">
                <img src="/images/photodune-7770665-two-white-coffee-mug-with-diy-decoration-o.jpg" class="card-img-top" alt="...">
                <div class="card-body">
                    <p>03 Dec 2023 / 0 Comments</p>
                    <h5 class="card-title">SEDIAL EIUSM TEMPOR</h5>
                    <p class="card-text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ratione, commodi? Repudiandae beatae omnis necessitatibus ea dicta quod, laudantium, expedita veritatis obcaecati consequuntur earum ipsam doloremque. Omnis atque voluptate dignissimos soluta..</p>
                    <a href="">Read More</a>
                </div>
            </div>

            <div class="card">
                <img src="/images/photodune-8797753-multiethnic-people-with-startup-business-t.jpg" class="card-img-top" alt="...">
                <div class="card-body">
                    <p>03 Dec 2023 / 2 Comments</p>
                    <h5 class="card-title">DONE LUCTUS IMPERDIET</h5>
                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Tempora provident veritatis vero accusamus consectetur maxime enim officia. Ea exercitationem suscipit veritatis eveniet maxime qui, dolores quia ipsam consequuntur repellendus distinctio.</p>
                    <a href="">Read More</a>
                </div>
            </div>

            <div class="card">
                <img src="/images/photodune-8522811-speaker-at-business-conference-and-present.jpg" class="card-img-top" alt="...">
                <div class="card-body">
                    <p>03 Dec 2023 / 2 Comments</p>
                    <h5 class="card-title">MAGNA PARS STUDIORUM</h5>
                    <p class="card-text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iure illo ipsum velit magni in? Vitae, maiores! A esse quos tempora aliquid, facere necessitatibus blanditiis nam repudiandae alias excepturi tenetur fuga!</p>
                    <a href="">Read More</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use '../style/main.scss'as *;


    .box {
        padding: 50px 0;

        .title {
            margin: 30px 0;
            .inline {
                display: flex;
                justify-content: space-between;
                align-items: center;
                width: 800px;

                h3 {
                    text-transform: uppercase;
                    font-weight: bold;
                    margin-right: 50px;
                }
            }

            a {
                color: $Scarlet;
                text-decoration: none;
                font-style: italic;
            }
        }

        .card{
            width: 25rem;
            border: none;
            .card-body{
                h5{

                }
                p{
                    font-size: 14px;
                    color: $Natural-Gray;
                }
                a{
                    color: $Scarlet;
                text-decoration: none;
                font-style: italic;
                }
            }
        }
    }
</style>