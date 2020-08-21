<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <form-helper>
      <h2 slot="title">I am the slot title</h2>
      <h3 slot="sec">I am the second one, huh?</h3>
    </form-helper>
  </div>
</template>

<script>
import formHelper from './components/formHelper.vue'

export default {
  components: {
    "form-helper":formHelper
  },
  data(){
    return{
      
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
