<template>
  <div class="calc">
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
.calc {
  width:500px;
  margin:2rem auto;
  display: grid;
  grid-template-columns: repeat(4,1fr);
  grid-auto-rows: minmax(50px,auto);
  font-size: 1.6rem;
  text-align: center;
  color:rgb(4, 4, 185);
  background-color: rgb(202, 201, 195);
}

.display{
  grid-column: 1/5;
  background-color: rgb(74, 79, 83);
  color:#fff;
  font-size: 40px;
  text-align: end;
}

.zero{
  grid-column:1/3;
}

.btn{
  border:3px solid #fff;
  padding: 3px;
  cursor: pointer;
}

.oper{
  background-color: orange;
}

</style>
