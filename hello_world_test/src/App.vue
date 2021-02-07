<template>
  <HelloWorld />
  <QrcodeVue/>
  
  
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import QrcodeVue from './components/QrCode'


export default {
  name: 'App',
  components: {
    HelloWorld,
    QrcodeVue,
    
   
  }
}
</script>

<style>
body {
  background-color: rgb(201, 179, 146);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  
  margin-top: 60px;
}

</style>
