<template>
  <div class="colorPickerContenedor">
    <h1>{{ msg }}</h1>
    <div class="colorPicker">
      <div class="puntero">
        <div class="forma1"></div>
      </div>
      <div class="bg bg1"></div>
      <div class="bg bg2"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Color Picker'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1 {
    font-weight: normal;
  }
  .colorPickerContenedor {
    margin: 10px;
    border: 1px solid #8E8E8E;
    //position: center;
    width: 240px ;
    height: 300px;
  }
  .colorPicker {
    margin: auto;
    width: 200px;
    height: 200px;
    background-color: #555;
  }
  .puntero {
    position: relative;
    z-index: 2;
    width: 8px;
  }
  .forma1 {
    margin-left: -9px;
    margin-top: -9px;
    width: 18px;
    height: 18px;
    border: 2px solid #000;
    -webkit-border-radius:9px ;
    -moz-border-radius: 9px;
    border-radius: 9px;
  }
  .bg {
    position: absolute;
    width: 100%;
    height: 100%;
  }
  .bg1 {
    z-index: 0;
    background: linear-gradient(to right, #fff 0%, rgba(255, 255, 255, 0) 100%);
  }
  .bg2{
    z-index: 1;
    background: linear-gradient(to bottom, transparent 0%, #000 100%);
  }
</style>
