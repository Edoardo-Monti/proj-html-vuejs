<script>
import SpeakerComp from './SpeakerComp.vue';
import TimerComp from './TimerComp.vue';
import UsComp from './UsComp.vue';

export default{
    name: "MainComp",
    components: { UsComp, TimerComp, SpeakerComp }
}

</script>

<template>
<UsComp/>
<TimerComp/>
<SpeakerComp/>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>
