<template>
  <div id="app">
    <Calc />
    <HelloWorld :msg="message" :myArr="arr" />
  </div>
</template>

<script>
import Calc from "./components/Calc.vue";
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Calc,
  },
  data: () => ({
    message: "",
  }),
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
