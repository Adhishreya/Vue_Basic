<template>
  <div>
    <h1>So why is Opensource contribution glorified so much?</h1>
    <h3>
      Let's hear it from <a href="https://octoverse.github.com/">OCTOVERSE</a>
    </h3>

    <h5>How many PRs have u made this October!!??</h5>
    <input
      increment="false"
      min="0"
      v-bind:style="inputs"
      v-on:input="accept"
      type="number"
      v-on:keyup.enter="inputs.value = $event.target.value"
    />
    <br />
    <button class="btn btn-primary" v-on:click="clicked">CLAIM REWARDS</button>
    <h3 v-if="reward">Congratulations!! You have finally made it ..</h3>
  </div>
</template>

<script>
export default {
  name: "Popular",
  data() {
    return {
      reward: false,
      inputs: {
        backgroundColor: "",
        color: "",
        value: 0,
      },
    };
  },
  methods: {
    clicked() {
      if (this.inputs.value > 0) {
        this.reward = true;
      }
    },
    accept() {
      // alert(val.value);
      this.inputs.backgroundColor = "gray";
      this.inputs.color = "black";
    },
  },
};
</script>


<style >
a {
  color: aquamarine;
}
body {
  background-color: rgb(64, 64, 64);
  color: aliceblue;
}
input {
  font-size: 25px;
  width: fit-content;
}
/* input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0; */
/* } */
</style>