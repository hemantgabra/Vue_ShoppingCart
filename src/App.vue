<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <Testing v-if="demo" @showTesting="showTesting($event)"></Testing>
    <!-- <button @click="showTesting">Click</button> -->
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Testing from "./components/Testing.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Testing
  },
  data() {
    return {
      demo: false
    };
  },
  methods: {
    showTesting() {
      this.demo = true;
    }
  }
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
