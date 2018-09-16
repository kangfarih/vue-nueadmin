<template>
<div id="app">
  <img alt="Vue logo" src="./assets/logo.png">
  <LoginPage></LoginPage>
</div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import LoginPage from "./components/LoginPage.vue";
// import VueRouter from 'vue-router';

export default {
  name: "app",
  components: {
    HelloWorld,
    LoginPage
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
