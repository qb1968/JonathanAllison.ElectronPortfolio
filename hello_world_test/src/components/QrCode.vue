<template>
  
 <div class="qr_codes">
 <h5 class="ja">Jonathan Allison</h5>
  <qrcode-vue  :value="value" :size="size" level="H" />
  <h5 class="tz">Tezos</h5>
  <qrcode-vue :value="value1" :size="size1" level="H" />
  <h5 class="bt">Burst</h5>
  <qrcode-vue :value="value2" :size="size2" level="H" />
  <h5 class="co">Cardano</h5>
  <qrcode-vue :value="value3" :size="size3" level="H" />
  </div>
</template>
<script>
  import QrcodeVue from 'qrcode.vue'

  export default {
    data() {
      return {
        value: 'https://github.com/qb1968',
        size: 50,
        value1: 'https://goldprice.org/cryptocurrency-price/tezos-price',
        size1: 50,
        value2: 'https://coinranking.com/coin/LUbkfWw7GwJ73+burstcoin-burst',
        size2: 50,
        value3: 'https://goldprice.org/cryptocurrency-price/cardano-price',
        size3: 50
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

}

h5 {
    font-size: 12px;
}


</style>