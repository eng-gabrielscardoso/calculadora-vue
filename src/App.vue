<template>
  <div id="app">
    <h1>{{title}}</h1>
    <Calculator></Calculator>
  </div>
</template>

<script>
import Calculator from './template/Calculator.vue';

export default {
  name: 'App',
  props: {},
  components: {
    Calculator
  },
  data: function() {
    return{
      title: 'Calculadora VueJS'
    }  ;
  }
}
</script>

<style>
  @font-face {
    font-family: 'Roboto';
    src: url('../public/assets/fonts/Roboto-Thin.ttf');
  }

  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Roboto', monospace;
  }

  html,
  body{
    height: 100%;
    overflow-x: hidden;
  }

  #app{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
    color: #FFFFFF;
    background-image: linear-gradient(to right, rgb(83,105,118), rgb(41,16,73));
  }
</style>
