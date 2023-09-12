<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld  :event='event' :msg="msg"/>
    <div>{{text}}</div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
export default {
  name: 'App',
   data(){
    return {
     msg:'Welcome to Your Vue.js App',
     event:{
      agree:(val)=>{
        this.hello(val)
      }
     }
    }
  },
  methods:{
    hello(val){
      this.text=val
    }
  },
  components: {
    HelloWorld
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
