<template>
  <div id="app">
    <HelloWorld
      msg="The pandemic has indeed brought the world to a standstill....... What are you doing to keep yourself on the run?........"
      ossd="OPEN SOURCE SOFTWARE DAYS"
    />
    <Popular />

    <button class="border-0" v-on:click="color">
      <h2 v-bind:style="back" id="caution">
        Warning: Site under construction!!
      </h2>
    </button>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import Popular from "./components/Popular";
import Goals from "./components/Goals";
export default {
  name: "App",
  components: {
    HelloWorld,
    Popular,
  },
  data() {
    return {
      back: {
        backgroundColor: "",
        color: "",
      },
    };
  },
  methods: {
    color() {
      alert("Work under progress!");

      this.back.backgroundColor = "red";
    },
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
#caution {
  color: beige;
  background: brown;
}
body {
  background-color: rgb(64, 64, 64);
}
</style>
