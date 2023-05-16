<script>
  export default {
    name: "TimerComp",
    data() {
      return {

      }
    },
    mounted() {
      // Set the date we're counting down to
      var countDownDate = new Date("Jan 5, 2024 15:37:25").getTime();

      // Update the count down every 1 second
      var x = setInterval(function () {

        // Get today's date and time
        var now = new Date().getTime();

        // Find the distance between now and the count down date
        var distance = countDownDate - now;

        // Time calculations for days, hours, minutes and seconds
        var days = Math.floor(distance / (1000 * 60 * 60 * 24));
        var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        var seconds = Math.floor((distance % (1000 * 60)) / 1000);

        // Output the result in an element with id="demo"
        // document.getElementById("demo").innerHTML = days + "d " + hours + "h " +
        //   minutes + "m " + seconds + "s ";

        document.getElementById("days").innerHTML = days;
        document.getElementById("hours").innerHTML = hours;
        document.getElementById("minutes").innerHTML = minutes;
        document.getElementById("seconds").innerHTML = seconds;

        // If the count down is over, write some text 
        if (distance < 0) {
          clearInterval(x);
          document.getElementById("days").innerHTML = "F";
          document.getElementById("hours").innerHTML = "I";
          document.getElementById("minutes").innerHTML = "N";
          document.getElementById("seconds").innerHTML = "E";
        }
      }, 1000);
    }
  }
</script>

<template>
  <div class="box text-center"> 
    <div class="d-flex justify-content-center align-items-center">
      <div id="days"></div>
      <div id="hours"></div>
      <div id="minutes"></div>
      <div id="contSeconds">
        <div id="seconds" class="animate__animated animate__flipOutX animate__infinite animate__slow">
        </div>
      </div>
    </div>

    <div id="email">
      <h4>SUBSCRIBE FOR UPDATE</h4>
      <div >
        <input type="email" placeholder="Please fill your email!" name="" id="">
        <button>SUBSCRIBE</button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @use '../style/main.scss'as *;

  .box {
    height: 500px;
    background-image: url(/images/coutdown-bg1.jpg);
    background-position-y: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    .d-flex{
      padding: 20px 0;
      #days {
        width: 100px;
        height: 100px;
        background-color: rgba(0, 0, 0, 0.5);
        margin-left: 30px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 40px;
        font-weight: bold;
        color: $White;
        border-radius: 5px;
      }
  
      #hours {
        width: 100px;
        height: 100px;
        background-color: rgba(0, 0, 0, 0.4);
        margin-left: 30px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 40px;
        font-weight: bold;
        color: $White;
        border-radius: 5px;
      }
  
      #minutes {
        width: 100px;
        height: 100px;
        background-color: rgba(0, 0, 0, 0.4);
        margin-left: 30px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 40px;
        font-weight: bold;
        color: $White;
        border-radius: 5px;
      }
  
      #contSeconds {
        width: 100px;
        height: 100px;
        background-color: rgba(0, 0, 0, 0.4);
        margin-left: 30px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 40px;
        font-weight: bold;
        color: $White;
        border-radius: 5px;
      }
    }
    #email{
      h4{
        padding: 20px 0;
      }
      input{
        height: 50px;
        width: 400px;
      }
      button{
        background-color: $Scarlet;
        color: $White;
        border: none;
        padding: 12px;
        margin-left: 30px;
      }
    }
  }
</style>