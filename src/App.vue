<template>
  <div app="app">
    <ul>
      <li>
        <router-link to="/">Home</router-link>
      </li>
      <li>
        <router-link to="demo1">Demo 1</router-link>
      </li>
      <li>
        <router-link to="demo2">Demo 2</router-link>
      </li>
    </ul>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "app",
  created() {},
  methods: {},
};
</script>

<style scoped>
ul {
  margin: 0;
  padding: 0;
}
li {
  display: inline;
  margin-right: 5px;
}
</style>
