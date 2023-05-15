<script>
export default{
  name: "LocationComp",
}

</script>

<template>
<div class="box text-center d-flex align-items-center justify-content-center">
        <div>
            <h1>LOCATION</h1>
            <p>GD BUILDING, GRAND CONFERENCE ROOM</p>
            <div>
                <i class="fa-regular fa-paper-plane"></i>
                <span>11 GD Building, River Mail, New York, USA 8879</span>
            </div>
            <p class="red">Check For Accomodation Here</p>
            <div>
                <img src="/images/1-item-2.jpg" alt="">
                <div class="d-flex justify-content-center">
                    <div class="mr-4">
                        <i class="fa-solid fa-phone"></i>
                        <span>+1-112-222-3344</span>
                    </div>
                   <div >
                    <i class="fa-solid fa-envelope"></i>
                    <span>contact@TheKeyNote.com</span>
                   </div>
                </div>
               
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

.box{
    height: 500px;
    background-image: url(/images/location-bg.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    color: $White;
    h1{
        font-weight: bold;
        padding: 10px 0;
    }
    p{
        font-size: 25px;
    }
    .red{
        font-size: 13px;
        margin: 20px 0;
        color: $Scarlet;
    }
}
</style>