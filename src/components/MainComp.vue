<script>
import ProgramComp from './ProgramComp.vue'
import SpeakerComp from './SpeakerComp.vue';
import TimerComp from './TimerComp.vue';
import UsComp from './UsComp.vue';
import {store} from '../store';
import ZoneComp from './ZoneComp.vue';
import NewsComp from './NewsComp.vue';


export default{
    name: "MainComp",
    components: { UsComp, TimerComp, SpeakerComp, ProgramComp, ZoneComp, NewsComp },
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
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>
