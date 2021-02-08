<template>
  <div class="hello">
    <h1>Hello World</h1>
    <button class="btn" onclick="window.print();">CLICK ME</button>

    <div class="container">
      <div class="head">
        <h2>Scan code to learn more about me</h2>
      </div>
      <div class="qr1">
        <h5 class>Jonathan Allison</h5>
        <img class="pic" src="../assets/qr-code.png" />
      </div>
      <div class="head1">
        <h2>Scan Code For Today's Pricing</h2>
      </div>
      <div class="qr_codes">
        <div class="qr1">
          <h5>Tezos Price</h5>
          <img class="pic" src="../assets/tezos.png" />
        </div>
        <div class="qr1">
          <h5 class="bt">Burst Price</h5>
          <img class="pic" src="../assets/burst.png" />
        </div>
        <div class="qr1">
          <h5 class="co">Cardano Price</h5>
          <img class="pic" src="../assets/cardano.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.btn {
  background-color: aqua;
}
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
  height: 200px;
  width: 200px;
}
</style>
