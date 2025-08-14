<template>
  <AppHeader 
  v-show="showHeader"/>

  <div v-show="ShowName">
    Nome:{{name}}
    Sobrenome:{{lastname}}
  </div>

  <div v-if = "acesslevel === 'admin' ">Admin</div>
  <div v-else-if = "acesslevel === 'marketing' ">Marketing</div>
  <div v-else>User</div>

  

  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    AppHeader
  },
  data(){
    return{
      showHeader:false,
      name : "joao",
      last : "silva",
      ShowName: false,
      acesslevel: 'admin'
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
}
</style>
