<template>
  <div class="hello">
    <!-- <h1>{{ msg }}</h1> -->
    <button @click="showTesting()">Click</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    demo: Boolean
  },
  methods: {
    showTesting() {
      let tDemo = this.demo;
      tDemo;
      this.$emit("showTesting", (tDemo = true));
      alert("hi");
      console.log(tDemo);
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
