<template>

    <footer>
        <h5>{{copyright}}</h5>
    </footer>


</template>

<script>


export default {
  data(){
      return{
          copyright:"Copyright of AbdulMalik Shareef Studio &copy;"
      }
  }
}
</script>

<style scoped>

footer{
    background: #222;
    padding:6px;
}

h5{
    color:lightgreen;
    text-align:center;
}


</style>
