<script>
export default{
  name: "UsComp",
}

</script>

<template>
<div>
    <div class="w-75 d-flex mx-auto p-5">
        <div class="d-flex">
            <div class="px-3">
                <i class="fa-solid fa-trophy"></i>
            </div>
            <div>
                <p class="title">WHO WE ARE</p>
                <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum! </p>
                <a href="">Learn More</a>
            </div>
        </div>
        <div class="d-flex">
            <div class="px-3">
                <i class="fa-solid fa-bolt"></i>
            </div>
            <div>
                <p class="title">WHAT WE DO</p>
                <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum! </p>
                <a href="">Learn More</a>
            </div>
        </div>
        <div class="d-flex">
            <div class="px-3">
                <i class="fa-solid fa-question"></i>
            </div>
            <div>
                <p class="title">why us</p>
                <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum! </p>
                <a href="">Learn More</a>
            </div>
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

div{
    i{
        font-family: "Font Awesome 6 Free";
        color: $Natural-Gray;
        font-size: 25px;
      
    }
}
div{
    .title{
        text-transform: uppercase;
        font-weight:bold;
    }
    .paragraph{
        font-size: 14px;
        padding: 15px 0;
        color: $Natural-Gray;
    }
    a{
        color: $Scarlet;
        text-decoration: none;
        font-style: italic;
    }
}

</style>