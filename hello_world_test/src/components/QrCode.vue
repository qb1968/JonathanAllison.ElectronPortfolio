<template>
<div class="container">
  <div class="head">
    <h2>Scan code to learn more about me</h2>
  </div>
<div class="qr1">
  <h5 class>Jonathan Allison</h5>
  <qrcode-vue  :value="value" :size="size" level="H" />
  </div>
<div class="head">
  <h2>Scan Code For Today's Pricing</h2>
</div>
<div class="qr_codes">
   
  
  <div class="qr1">
  <h5>Tezos Price</h5>
 
  <qrcode-vue :value="value1" :size="size1" level="H" />
  </div>
  <div class="qr1">
  <h5 class="bt">Burst Price</h5>
  <qrcode-vue :value="value2" :size="size2" level="H" />
  </div>
  <div class="qr1">
  <h5 class="co">Cardano Price</h5>
  <qrcode-vue :value="value3" :size="size3" level="H" />
</div>
</div>
</div>   
</template>
<script>
  import QrcodeVue from 'qrcode.vue'
  

  
  export default {
    data() {
      return {
        value: 'https://thejonathanallison.com',
        size: 150,
        value1: 'https://goldprice.org/cryptocurrency-price/tezos-price',
        size1: 150,
        value2: 'https://coinranking.com/coin/LUbkfWw7GwJ73+burstcoin-burst',
        size2: 150,
        value3: 'https://goldprice.org/cryptocurrency-price/cardano-price',
        size3: 150
      }
    },
    components: {
      QrcodeVue,
      
      
      
    },
  }
</script>

<style>
.container {
  background-color: aqua;
}
.qr_codes {
    display: flex;
    justify-content: space-evenly;
    padding: 1rem;
    
    
    

}
.qr1 {
    align-content: center;
}
h5 {
    font-size: 16px;
}



</style>