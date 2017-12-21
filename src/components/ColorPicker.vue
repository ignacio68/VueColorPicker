<template>
  <div class="todo">
    <div class="colorPickerContenedor">
      <div class="colorPicker"></div>
      <div class="slider"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ColorPicker',
  data() {
    return {

     }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.todo {
  width: 600px;
}
  .colorPickerContenedor {
    width: 100%;
    padding-bottom: 120%;
    border: 1px solid;
  }
  .colorPicker {
  /*  width: 100%;
  /*  height:80%;*/
  /*  position: absolute;*/
    top: 0px;
    left: 0px;
    width: 100%;
    padding-bottom: 90%;
    border: 2px solid red;
    /*background-color: red;*/
  }
  .slider {
    width: 100%;
    padding-bottom: 10%;
    border: 2px solid green;
  }

</style>
