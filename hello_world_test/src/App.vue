<template>
  <HelloWorld />
  <QrcodeVue />
  <TwitterFeed />
  <Footer />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import QrcodeVue from "./components/QrCode";
import TwitterFeed from "./components/TwitterFeed";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    HelloWorld,
    QrcodeVue,
    TwitterFeed,
    Footer,
  },
};
</script>

<style>
body {
  background-color: rgb(219, 180, 122);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;

  margin-top: 20px;
}
</style>
