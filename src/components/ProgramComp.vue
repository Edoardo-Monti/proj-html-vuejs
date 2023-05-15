<script>
import {store} from '../store';

  export default {
    name: "ProgramComp",

    data(){
      return{
        store,
        array:[
          {
            day: "DAY 1",
            date: "24-04-2023",
            info: [
              {
                orario: "09:00 - 10:30",
                stanza: "Room A",
                nome: "laurence Francis",
                intro: "WELCOMING AND INTRODUCTION",
                para: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum",
                img: "/images/speaker-2.jpg"
              }
          ]
            
          },
          {
            day: "DAY 2",
            date: "25-04-2023",
            info:[
              {
                orario: "09:00 - 10:30",
                stanza: "Room B",
                nome: "Jone Jones",
                intro: "THE WORLD OF WORK",
                para: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum",
                img: "/images/speaker-3.jpg"
              }
              ] 
          },
          {
            day: "DAY 3",
            date: "26-04-2023",
            info: [
              {
                orario: "09:00 - 10:30",
                stanza: "Room C",
                nome: "Ugo Foscolo",
                intro: "POESIE",
                para: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum",
                img: "/images/speaker-4.jpg"
              }
            ]
          },
          {
            day: "DAY 4",
            date: "27-04-2023",
            info:[
              {
                orario: "09:00 - 10:30",
                stanza: "Room D",
                nome: "Pirata",
                intro: "HOW TO IMPROVE",
                para: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum",
                img: "/images/speaker-5.jpg"
              }
            ] 
          },
          {
            day: "DAY 5",
            date: "28-04-2023",
            info:[
              {
                orario: "09:00 - 10:30",
                stanza: "Room E",
                nome: "Edoardo Monti",
                intro: "WORK ON YOU FIRST",
                para: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum",
                img: "/images/speaker-6.jpg"
              }
            ]
          },
          {
            day: "DAY 6",
            date: "29-04-2023",
            info: [
              {
                orario: "09:00 - 10:30",
                stanza: "Room F",
                nome: "Andre felici",
                intro: "END MEATINGS",
                para: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda illo error eligendi aliquam fugit quisquam sequi eaque blanditiis voluptatum",
                img: "/images/speaker-7.jpg"
              }
            ]
          },
        ]
      }
    }
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

    <div class="date d-flex w-75 mx-auto mt-5 mb-5">
      <div class="col-2" v-for="(elem, index) in array" :key="index" @click="store.number = index" >
        <p>{{ elem.day }}</p>
        <p>{{ elem .date}}</p>
      </div>
      <!-- <div class="col-2">
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
      </div> -->
    </div>

    <div class="d-flex justify-content-around align-items-center w-75 mx-auto orario" v-for="(element, index) in array" :key="index" >
      <div v-if="index == store.number" class="col-2">
        <div class="d-flex align-items-center">
          <i class="fa-regular fa-clock"></i>
          <p>{{element.info[0].orario}}</p>
        </div>
        <div class="d-flex align-items-center">
          <i class="fa-solid fa-paper-plane"></i>
          <p>{{element.info[0].stanza}}</p>
        </div>
        <div class="d-flex align-items-center">
          <i class="fa-solid fa-user"></i>
          <p>{{element.info[0].nome}}</p>
        </div>
      </div>

      <div class="info col-8" v-if="index == store.number">
        <h4>
          {{element.info[0].intro}}
        </h4>
        <p>{{element.info[0].para}}</p>
        <img :src="element.info[0].img" alt="">
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
        font-size: 14px;
        padding: 15px 0;
        color: $Natural-Gray;
      }
      img{
        width: 50px;
      }
    }
    .orario{
      .col-2{
        div{
          i{
            font-family: "Font Awesome 6 Free";
            margin-right: 10px;
          }
        }
      }
    }
  }
</style>