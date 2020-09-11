<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <ChenMe msg="今天吃什么">
      <template>
        <div>hello</div>
      </template>
    </ChenMe>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import ChenMe from './components/ChenMe.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    ChenMe
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
  font-size: 12px;
}
</style>
