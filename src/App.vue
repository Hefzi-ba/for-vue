<template>
  
  <CicloFor></CicloFor>
  <RawHtml/>
 <BdeNumeros/>
 <VforComp/>   
 
</template>

<script>
import CicloFor from './components/CicloFor.vue';
import RawHtml from './components/RawHtml.vue';
import BdeNumeros from './components/BdeNumeros.vue';
import VforComp from './components/VforComp.vue';



export default {
  name: 'App',
  components: {
    CicloFor,
    RawHtml,
    BdeNumeros,
    VforComp
}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
