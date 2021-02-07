<template>
  
<div class="qr_codes">
<div class="qr1">
  <h5 class>Jonathan Allison</h5>
  <qrcode-vue  :value="value" :size="size" level="H" />
  </div>
  <div class="qr1">
  <h5 class="tz">Tezos Price</h5>
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
   
</template>
<script>
  import QrcodeVue from 'qrcode.vue'
  

  
  export default {
    data() {
      return {
        value: 'https://github.com/qb1968',
        size: 60,
        value1: 'https://goldprice.org/cryptocurrency-price/tezos-price',
        size1: 60,
        value2: 'https://coinranking.com/coin/LUbkfWw7GwJ73+burstcoin-burst',
        size2: 60,
        value3: 'https://goldprice.org/cryptocurrency-price/cardano-price',
        size3: 60
      }
    },
    components: {
      QrcodeVue,
      
      
      
    },
  }
</script>

<style>

.qr_codes {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    padding: 1rem;
    margin-bottom: 20px;
    

}
.qr1 {
    align-content: center;
}
h5 {
    font-size: 12px;
}


</style>