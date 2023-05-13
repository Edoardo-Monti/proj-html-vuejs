<script>
import TimerComp from './TimerComp.vue';
import UsComp from './UsComp.vue';

export default{
    name: "MainComp",
    components: { UsComp, TimerComp }
}

</script>

<template>
<UsComp/>
<TimerComp/>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>
