<template>
  <div id="app">
    <HelloWorld
      msg="The pandemic has indeed brought the world to a standstill....... What are you doing to keep yourself on the run?........"
    />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #c6d4e2;

  margin-top: 60px;
}
body {
  background-color: rgb(64, 64, 64);
}
</style>
