<template>
  <div id="id">
    <img src="./assets/logo.png" alt="Vue logo">
    <Calculator msg="Vue js Calculator project"/>
  </div>
</template>

<script>
import Calculator from './components/Calculator.vue'

export default {
  name: 'App',
  components: {
    Calculator
  }
}
</script>

<style scoped>

</style>
