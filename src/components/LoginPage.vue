<template>
<div id="LoginPage">
  <h1>This is LoginPage</h1>
  <!-- <HelloWorld msg='Title'></HelloWorld> -->
  <div ref="hello">hellow <strong>gaes</strong></div>
  <p>{{this.output}}</p>
  <input type="text" ref="input">
  <button v-on:click="readRefs">Ref Button</button>
</div>
</template>

<script>
import HelloWorld from "./HelloWorld.vue";
export default {
  name: "LoginPage",
  components: {
    HelloWorld
  },
  data: function () {
    return {
      output: "Your favorite",
    }
  },
  methods: {
    readRefs: function () {
      console.log(this.$refs);
      this.output = this.$refs.input.value;
    }
  }
};
</script>
