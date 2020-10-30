<template>
  <div id="app">
    <HelloWorld
      msg="The pandemic has indeed brought the world to a standstill....... What are you doing to keep yourself on the run?........"
      ossd="OPEN SOURCE SOFTWARE DAYS"
    />
    <Popular />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Popular from "./components/Popular";

export default {
  name: "App",
  components: {
    HelloWorld,
    Popular,
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
