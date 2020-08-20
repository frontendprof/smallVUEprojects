<template>
  <div class="calc">
    <h1>{{msg}}</h1>
    <div class="basic-calc">

      <div class="display">{{current ||"0"}}</div>
      <div @click="clear" class="btn">C</div>
      <div @click="sign" class="btn">+/-</div>
      <div class="btn">%</div>
      <div class="btn oper">&divide;</div>
      <div class="btn">7</div>
      <div class="btn">8</div>
      <div class="btn">9</div>
      <div class="btn oper">&times;</div>
      <div class="btn">4</div>
      <div class="btn">5</div>
      <div class="btn">6</div>
      <div class="btn oper">&mdash;</div>
      <div class="btn">1</div>
      <div class="btn">2</div>
      <div class="btn">3</div>
      <div class="btn oper">+</div>
      <div class="btn zero">0</div>
      <div class="btn">.</div>
      <div class="btn oper">=</div>

    </div>
  
    
  </div>
</template>

<script>
export default {
  data(){
    return{
      current:"123"
    }
  },
  methods:{

    clear(){
      this.current="";
    },

    sign(){
      this.current=this.current.charAt(0)==="-"?this.current.slice(1):`${this.current}`
    }
  }
  
}
</script>

<style scoped>

.basic-calc{
  display: grid;
  grid-template-columns: repeat(4,1fr);
  grid-auto-rows: minmax(50px,auto);
  margin:0 auto;
  width: 400px;
}


</style>
