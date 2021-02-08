<template>
  <div class="hello">
    <h1>Hello World</h1>
    <button class="btn" onclick="window.print();">CLICK ME</button>
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
</style>
