<template>
  <img alt="Vue logo" src="./assets/boji.png">
  <!--  <HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <br>
  <CountDemo/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import CountDemo from "@/components/CountDemo";

export default {
  name: 'App',
  components: {
    CountDemo
    // HelloWorld
  }
}
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
