<template>
  <div class="calculator">
    <Display></Display>
    <Button></Button>
    
  </div>
</template>

<script>
import Button from '../components/Button.vue';
import Display from '../components/Display.vue';

export default {
  name: 'Calculator',
  props: {},
  components: {
    Button,
    Display
  },
  data: function() {
    return{};
  }
}
</script>

<style scoped>
  .calculator{
    display: grid;
    grid-template-columns: repeat(4, 25%);
    grid-template-rows: 1fr 48px 48px 48px 48px 48px;
    height: 320px;
    width: 235px;
    border-radius: 5px;
    overflow: hidden;
  }
</style>