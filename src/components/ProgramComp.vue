<script>
  export default {
    name: "ProgramComp",

  }
</script>

<template>
  <div class="box">
    <div class="title w-75 mx-auto d-flex justify-content-between align-items-center">
      <div class="inline">
        <h3>SPEAKERS</h3>
        <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi
          aliquam fugit quisquam sequi eaque blanditiis voluptatum! </p>
      </div>
      <a href="">Learn More</a>
    </div>

    <div class="date d-flex w-75 mx-auto mt-5">
      <div class="col-2">
        <p>DAY 1</p>
        <p>24-04-2023</p>
      </div>
      <div class="col-2">
        <p>DAY 2</p>
        <p>25-04-2023</p>
      </div>
      <div class="col-2">
        <p>DAY 3</p>
        <p>26-04-2023</p>
      </div>
      <div class="col-2">
        <p>DAY 4</p>
        <p>27-04-2023</p>
      </div>
      <div class="col-2">
        <p>DAY 5</p>
        <p>28-04-2023</p>
      </div>
      <div class="col-2">
        <p>DAY 6</p>
        <p>29-04-2023</p>
      </div>
    </div>

    <div class="d-flex justify-content-around w-75 mx-auto mt-5">
      <div>
        <div class="d-flex">
          <i class="fa-regular fa-clock"></i>
          <p>09:00 - 10:30</p>
        </div>
        <div class="d-flex">
          <i class="fa-solid fa-paper-plane"></i>
          <p>Room A</p>
        </div>
        <div class="d-flex">
          <i class="fa-solid fa-user"></i>
          <p>Laurence Francis</p>
        </div>
      </div>

      <div class="info">
        <h4>
          WELCOMING AND INTRODUCTION
        </h4>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae eos eaque ratione amet quibusdam nihil enim animi mollitia suscipit atque sunt id ab hic aut laboriosam voluptas, repellat veniam non.</p>
        <img src="/images/speaker-2.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @use '../style/main.scss'as *;

  .box {
    padding: 50px 0;
    .title {

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

        .paragraph {
          font-size: 14px;
          padding: 15px 0;
          color: $Natural-Gray;
        }

      }

      a {
        color: $Scarlet;
        text-decoration: none;
        font-style: italic;
      }
    }
    .date{
      .col-2{
        background-color: $Scarlet;
        padding: 10px;
        border-left: 1px solid $Masala;
        cursor: pointer;
        &:hover{
          background-color: $Thunderbird;
        }
        p{
          font-weight: bold;
          &:nth-child(2){
            font-size: 12px;
          }
        }
      }
    }

    .info{
      h4{

      }
      p{

      }
      img{
        width: 50px;
      }
    }
  }
</style>