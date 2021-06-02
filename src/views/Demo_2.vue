<template>
  <div app="demo2">
    <h1>Demo#2</h1>
    <button v-on:click="clickMe">ClickMe</button>
    <button @click="clickMe2(`Hello`)">ClickMe 2</button>
  </div>
</template>

<script>
export default {
  name: "Demo2",
  data() {
    return {};
  },
  mounted() {
    this.initial();
  },
  methods: {
    initial() {
      console.log("initial");
    },
    clickMe() {
      alert("Hi");
    },
    clickMe2(message) {
      alert(message);
    },
  },
};
</script>
