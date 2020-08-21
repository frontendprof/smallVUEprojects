<template>
  <div id="app">
    <img alt="Vue logo" id="imgFile" src="./assets/logo.png">
    <form-helper>

      <div slot="form-header">
        <h3>This is the title of the form</h3>
        <p>Information about the form</p>
      </div>

      <div slot="form-fields">
        <input type="text" placeholder="Name" required>
        <input type="password" placeholder="Password" required>
      </div>


      <div slot="form-controls">
        <button class="btn btn-large btn-success" v-on:click="handleSubmit">Submit</button>
        
      </div>


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
      title:"I am the slot title from data function"
      
    }
  },

  methods:{
    handleSubmit:function(){
      alert("Thanks for submitting")
    }
  }
}
</script>

<style>

#app { 
  text-align: center;
  color: #2c3e50;
  margin-top: 5px;
  position: relative;
}

#imgFile{
  height: 10rem;
  position: absolute;
  right:20px;
  top:14rem;
}
</style>
