<script>
export default{
  name: "SingleTicket",
  props: ['propsTicket']
}

</script>

<template>
<div class="ticket">
    <div class="uno">
        <h4>{{ propsTicket.title }}</h4>
        <p>{{ propsTicket.cost }}</p>
    </div>
    <div class="due ">
        <p>{{ propsTicket.vantage1}}</p>
        <p>{{ propsTicket.vantage2}}</p>
        <p>{{ propsTicket.vantage3}}</p>
        <p>{{ propsTicket.vantage4}}</p>
        <p>{{ propsTicket.vantage5}}</p>
    </div>
    <div>
        <button>Book Now</button>
    </div>
</div>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

.ticket{
    width: 20rem;
    padding: 50px 0;
    text-align: center;
    .uno{
        padding: 20px 0;
        background-color: $Cloud;
        h4{
            
            font-size: 20px;
        }
        p{
            color: $Thunderbird;
        }
    }
    .due{
        background-color: $White;
        padding: 30px 0;
        p{
            font-size: 14px;
            color: $Natural-Gray;
            font-style: italic;
        }
        
    }
    button{
            width: 100%;
            border: none;
            background-color: $Scarlet;
            color: $White;
            padding: 10px 0;
        }

}
</style>