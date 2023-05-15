<script>
import MapComp from './MapComp.vue';
import LocationComp from './LocationComp.vue'

export default{
    name: "ZoneComp",
    components: { MapComp,LocationComp }
}

</script>

<template>
<MapComp/>
<LocationComp/>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>