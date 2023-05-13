<script>
export default{
  name: "JumboComp",
}

</script>

<template>
    <div class="box text-center">
        <div>
            <p>CONFERENCE ON</p>
            <h1>SOCIAL NETWORKS</h1>
            <div>
                <img src="/images/1-item-2.jpg" alt="">
                <div class="d-flex justify-content-center">
                    <span>23 - 26 May 2023</span>
                    <span>/</span>
                    <span>SAN FRANCISCO</span>
                    <span>/</span>
                    <span>8 SPEAKERS</span>
                </div>
                <button type="button" class="btn btn-danger">REGISTER ONLINE</button>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

.box{
    height: 600px;
    background-image: url(/images/slider-1-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position-y: center;
    display: flex;
    justify-content: center;
    align-items: center;
    div{
        p{
            font-size: 50px;
            color: $Natural-Gray;
        }
        h1{
            font-size: 90px;
            font-weight: bold;
            color: $White;
        }
        div{
            color: $White;
            span{
                margin: 0 15px;
            }
        }
        button{
            margin-top: 30px;
            padding: 10px 15px;
        }
    }
}
</style>