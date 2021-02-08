<template>
  <div class="container">
    <div class="head">
      <h2>Scan code to learn more about me</h2>
    </div>
    <div class="qr1">
      <h5 class>Jonathan Allison</h5>
      <img class="pic" src="../assets/qr-code.png"/> 
    </div>
    <div class="head1">
      <h2>Scan Code For Today's Pricing</h2>
    </div>
    <div class="qr_codes">
      <div class="qr1">
        <h5>Tezos Price</h5>
        <img class="pic" src="../assets/tezos.png"/>
      </div>
      <div class="qr1">
        <h5 class="bt">Burst Price</h5>
         <img class="pic" src="../assets/burst.png"/>
      </div>
      <div class="qr1">
        <h5 class="co">Cardano Price</h5>
        <img class="pic" src="../assets/burst.png"/>
      </div>
    </div>
  </div>
</template>
<script>


export default {
  data() {
    return {
      ref:"./assets/qr-code",
      value: "http://thejonathanallison.com",
      size: 150,
      value1: "https://goldprice.org/cryptocurrency-price/tezos-price",
      size1: 150,
      value2: "https://coinranking.com/coin/LUbkfWw7GwJ73+burstcoin-burst",
      size2: 150,
      value3: "https://goldprice.org/cryptocurrency-price/cardano-price",
      size3: 150,
    };
  },
  components: {
    QrcodeVue,
  },
};
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
.head1 {
  padding: 5px;
}
.pic {
  height:200px;
  width:200px;
}
</style>
