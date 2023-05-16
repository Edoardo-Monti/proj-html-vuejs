<script>
import ImgComp from './ImgComp.vue'

  export default {
    name: "FooterComp",
    components: { ImgComp },
    data(){
      return{
        arrayImg:[
          {
            img: "/images/6426608875_186070f8ca_o-150x150.jpg",
          },
          {
            img: "/images/13349065283_64d09b067c_o-150x150.jpg",
          },
          {
            img: "/images/apple-touch-icon-72x72-precomposed.png",
          },
          {
            img: "/images/19561693_60x60.jpg",
          },
          {
            img: "/images/card01-150x150.jpg",
          },
          {
            img: "/images/card04-150x150.jpg",
          },
          {
            img: "/images/photodune-6745579-modern-creative-man-relaxing-on-workspace-.jpg",
          },
          {
            img: "/images/photodune-6745606-man-wristwatch-calendar-key-and-glasses-on.jpg",
          },
          {
            img: "/images/photodune-8795110-overhead-of-essentials-denim-clothes-m-150.jpg",
          },
          {
            img: "/images/photodune-8523683-speaker-at-business-convention-and-present.jpg",
          },
          {
            img: "/images/photodune-8797753-multiethnic-people-with-startup-business-t (1).jpg",
          },
          {
            img: "/images/photodune-8522811-speaker-at-business-conference-and-present (1).jpg",
          },

        ]
      }
    }
  }
</script>

<template>
  <div class="bg-black">
    <div class="w-75 mx-auto d-flex justify-content-between">
      <div id="about">
        <h5>ABOUT US</h5>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. At, hic nostrum, eaque exercitationem ut quisquam
          corporis </p>
        <div class="d-flex justify-content-between">
          <i class="fa-brands fa-square-facebook"></i>
          <i class="fa-brands fa-square-twitter"></i>
          <i class="fa-brands fa-linkedin"></i>
          <i class="fa-brands fa-square-google-plus"></i>
          <i class="fa-brands fa-square-pinterest"></i>
        </div>
      </div>
      <div id="news">
        <h5>RECENT NEWS</h5>
        <ul>
          <li>SEM PORTE LA SPESA FUORA</li>
          <li>SEM PORTE LA SPESA FUORA</li>
          <li>SEM PORTE LA SPESA FUORA</li>
          <li>SEM PORTE LA SPESA FUORA</li>
          <li>SEM PORTE LA SPESA FUORA</li>
        </ul>
      </div>
      <div id="seat">
        <h5>GET YOUR SEAT</h5>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. At, hic nostrum, eaqu</p>
        <button>CHECK OUT TICKETS!</button>
      </div>
      <div id="gallery">
        <h5>GALLERY FROM LAST YESR</h5>
        <div class="cont-img">
            <ImgComp v-for="(elem, index) in arrayImg" :propsImg="elem"/>
        

        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @use '../style/main.scss'as *;

  .bg-black {
    padding: 50px 0;
    #about{
      width: 20%;
      h5{
        color: $White;
        font-size: medium;
        margin-bottom: 25px;
      }
      p {
        
        font-size: 14px;
        color: $Natural-Gray;
      }
      i{
        color: white;
        font-size: 25px;
      }
    }
    #news{
      width: 20%;
      h5{
        color: $White;
        font-size: medium;
        margin-bottom: 25px;
      }
      li{
        list-style-type: disc;
        font-size: 14px;
        color: $Natural-Gray;
      }
    }
    #seat{
      width: 20%;
      h5{
        color: $White;
        font-size: medium;
        margin-bottom: 25px;
      }
      p {
        
        font-size: 14px;
        color: $Natural-Gray;
      }
      button{
        font-size: 13px;
        padding: 15px;
        border: none;
        color: $White;
        background-color: $Scarlet;
      }
    }
    #gallery{
      width: 20%;
      h5{
        color: $White;
        font-size: medium;
        margin-bottom: 25px;
      }
      .cont-img{
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        gap: 6px;
        
      }
    }
  }
</style>