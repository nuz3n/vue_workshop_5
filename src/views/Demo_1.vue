<template>
  <div>
    <h1>Demo 1</h1>
    <h2>{{ this.$store.state.count }}</h2>
    <!-- <button @click="count++">Count</button> -->
    <!-- <br />
    <input type="text" v-model="message" />
    <br />
    {{ message }}
    <br /> -->
    <!-- <button @click="message = ''">Reset</button> -->

    <button @click="increment">Count</button>
  </div>
</template>

<script>
export default {
  name: "demo1",
  data() {
    return {
      title: "workshop #5",
      count: 0,
      message: "",
    };
  },
  methods: {
    increment() {
      this.$store.commit("increment");
      console.log(this.$store.state.count);
    },
  },
};
</script>

<style></style>
