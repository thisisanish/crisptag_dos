<template>
  <input type="text" v-on:change="UpperCase" />

  <h2>{{msg}}</h2>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      msg: "Enter Value and Press Enter",
    };
  },
  methods: {
    UpperCase(e) {
      this.msg = e.target.value.toUpperCase();
    },
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
</style>
