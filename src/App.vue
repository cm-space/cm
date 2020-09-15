<template>
  <div id="app">
<!--    <img alt="Vue logo" src="./assets/logo.png">-->
    <transition name="fade" key="0">
      <HelloWorld msg="Welcome to Your Vue.js App" v-show="show"></HelloWorld>
    </transition>
    <ChenMe @switchShow="switchShow">
    </ChenMe>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import ChenMe from './components/ChenMe.vue';

export default {
  name: 'App',
  data(){
    return {
      msg:'hello',
      show:true
    }
  },
  components: {
    HelloWorld,
    ChenMe
  },
  methods:{
    switchShow(){
      this.show=!this.show
    }
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
.fade-enter-active, .fade-leave-active {
  transition: opacity 1s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}

</style>
