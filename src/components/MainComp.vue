<script>
import ProgramComp from './ProgramComp.vue'
import SpeakerComp from './SpeakerComp.vue';
import TimerComp from './TimerComp.vue';
import UsComp from './UsComp.vue';


export default{
    name: "MainComp",
    components: { UsComp, TimerComp, SpeakerComp, ProgramComp }
}

</script>

<template>
<UsComp/>
<TimerComp/>
<SpeakerComp/>
<ProgramComp/>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>
