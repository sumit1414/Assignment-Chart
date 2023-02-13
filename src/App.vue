<template>
  <div class="h-screen bg-f4f5f6">
    <ChartUI />
    <!-- <HelloWorld /> -->
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import ChartUI from "./components/ChartUI.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    ChartUI,
  },
};
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
.bg-f4f5f6 {
  background: #f4f5f6;
}
</style>
