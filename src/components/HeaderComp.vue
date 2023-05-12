<script>
import NavComp from './Nav.vue'

export default{
  name: "HeaderComp",
  components:{
    NavComp,
  }
}

</script>

<template>
<NavComp/>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;


</style>
