<template>
  <div class="calc">
    <div class="display">34343434</div>
    <div class="btn">C</div>
    <div class="btn">+/-</div>
    <div class="btn">%</div>
    <div class="btn oper">&divide;</div>
    <div class="btn">7</div>
    <div class="btn">8</div>
    <div class="btn">9</div>
    <div class="btn oper">&times;</div>
    <div class="btn">4</div>
    <div class="btn">5</div>
    <div class="btn">6</div>
    <div class="btn oper">-</div>
    <div class="btn">1</div>
    <div class="btn">2</div>
    <div class="btn">3</div>
    <div class="btn oper">+</div>
    <div class="btn zero">0</div>
    <div class="btn">.</div>
    <div class="btn">=</div>
    
  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.calc {
  display: grid;
  grid-template-columns: repeat(4,1fr);
  grid-auto-rows: minmax(50px,auto);
  font-size: 1.5rem;
  text-align: center;
  color:rgb(4, 4, 185);
  background-color: rgb(253, 223, 125);
}

.display{
  grid-column: 1/5;
  background-color: rgb(157, 167, 219);
  color:#fff;
  font-size: 40px;
  border:3px solid red;
}

.zero{
  grid-column:1/3;
}

.btn{
  border:3px solid #fff;
  padding: 3px;
}

</style>
