<script >
import {store} from './store';
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';


export default{
  name: 'App',
  components: {
    MainComp,
    HeaderComp,
    FooterComp,
},
  data(){
    return{
      store
    }
  }
}

</script>

<template>
  <div>
    <HeaderComp/>
    <MainComp/>
    <FooterComp/>
  </div>
</template>

<style lang="scss">
@use './style/main.scss' as *;

</style>
