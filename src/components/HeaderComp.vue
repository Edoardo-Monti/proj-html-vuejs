<script>
import JumboComp from './JumboComp.vue';
import NavComp from './Nav.vue'

export default{
  name: "HeaderComp",
  components:{
    NavComp,
    JumboComp
}
}

</script>

<template>
<NavComp/>
<JumboComp/>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>
