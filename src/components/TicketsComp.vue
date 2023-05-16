<script>
import SingleTicket from './SingleTicket.vue';

export default{
    name: "TicketsComp",
    components: { SingleTicket },
    data(){
        return{
            arrayTicket:[
                {
                    title: "ONE DAY PASS",
                    cost: "FREE",
                    vantage1: "One Day Access",
                    vantage2: "Coffe Break",
                    vantage3: "Lunch(International Buffet)",
                    vantage4: "Document Sheet",
                    vantage5: "50USD Voucher For Next Event",
                },
                {
                    title: "FOUR DAY PASS",
                    cost: "750.00 USD",
                    vantage1: "Four Day Access",
                    vantage2: "Coffe Break",
                    vantage3: "Lunch(International Buffet)",
                    vantage4: "Document Sheet",
                    vantage5: "100USD Voucher For Next Event",
                },
                {
                    title: "TWO DAY PASS",
                    cost: "580.00 USD",
                    vantage1: "Two Day Access",
                    vantage2: "Coffe Break",
                    vantage3: "Lunch(International Buffet)",
                    vantage4: "Document Sheet",
                    vantage5: "70USD Voucher For Next Event",
                },
            ]
        }
    }
}

</script>

<template>
    <div id="box">
        <h4 class="text-center">TICKETS</h4>
        <div class="w-75 mx-auto d-flex justify-content-between">
            
            <SingleTicket v-for="(elem, index) in arrayTicket" :propsTicket="elem"/>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

#box{
    padding: 50px 0;
    background-image:url(/images/ticket-bg.jpg) ;
    background-size: cover;
    h4{
        font-size: 30px;
        color: $White;
    }
}
</style>