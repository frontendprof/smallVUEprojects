<template>
  <div class="hello">
   
    <h1>Please fill out the form ...</h1>
    <form>
      <div id="form-header">
        <slot name="form-header"></slot>
      </div>
      <div id="form-fields">
        <slot name="form-fields"></slot>

      </div>
      <div id="form-controls">
        <slot name="form-controls"></slot>

      </div>
      <div id="useful-links">
        <ul>
          <li><a href="#">Link 1</a></li>
          <li><a href="#">Link 2</a></li>
          <li><a href="#">Link 3</a></li>
          <li><a href="#">Link 4</a></li>
          <li><a href="#">Link 5</a></li>
        </ul>
      </div>
    </form>


   
  </div>
</template>

<script>
export default {
  components:{

  },
  data(){
    return{

    }
  },

  methods:{

  }
}
</script>

<style scoped>
h1{
    text-align: center;
    color:rgb(95, 202, 130);
}
form{
    width: 100%;
    max-width: 960px;
    margin: 0 auto;
}
#useful-links ul{
    padding: 0;
}
#useful-links li{
    display: inline-block;
    margin-right: 5rem;
}
form > div{
    padding: 20px;
    background: rgb(223, 219, 219);
    margin: 20px 0;
    
}
#form-header{
    background: #ddd;
    border: 1px solid #bbb;
}
</style>
