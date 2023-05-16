<script>
import ProgramComp from './ProgramComp.vue'
import SpeakerComp from './SpeakerComp.vue';
import TimerComp from './TimerComp.vue';
import UsComp from './UsComp.vue';
import {store} from '../store';
import ZoneComp from './ZoneComp.vue';
import NewsComp from './NewsComp.vue';
import TicketsComp from './TicketsComp.vue';
import Presentation from './Presentation.vue';
import SponsorComp from './SponsorComp.vue';


export default{
    name: "MainComp",
    components: { UsComp, TimerComp, SpeakerComp, ProgramComp, ZoneComp, NewsComp, TicketsComp, Presentation, SponsorComp },
    data(){
        return{
            store
        }
    }
}

</script>

<template>
<UsComp/>
<TimerComp/>
<SpeakerComp/>
<ProgramComp/>
<ZoneComp/>
<NewsComp/>
<TicketsComp/>
<Presentation/>
<SponsorComp/>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>
