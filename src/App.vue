<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <Testing v-if="demo" @showTesting="this.demo = true"></Testing>
    <!-- <button @click="showTesting">Click</button> -->
    {{ name }}
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
      demo: false,
      name: "hemant"
    };
  }
  // methods: {
  //   showTesting() {
  //     this.demo = true;
  //     //console.log("done");
  //   }
  // }
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
