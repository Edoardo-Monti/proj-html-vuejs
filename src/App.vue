<script >
import {store} from './store';
import MainComp from './components/MainComp.vue';


export default{
  name: 'App',
  components: {
    MainComp,
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
    <h1 class="animate__animated animate__rubberBand">ciao</h1>
    
    <MainComp/>
  </div>
</template>

<style lang="scss">
@use './style/main.scss' as *;

div{
  
  h1{
    color: $Gray;
  }
}
</style>
