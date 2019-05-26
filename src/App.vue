<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloTime />
    <HelloWorld msg="欢迎来到程序员工具大全"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HelloTime from './components/HelloTime.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    HelloTime
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
