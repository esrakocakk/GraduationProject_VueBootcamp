<script setup>
import Button from "../src/components/Button/Button.vue"
</script>

<template>
  <div class="included">

    <div class="finish" id="finish"></div>
    
    <img id="atbir" src="../src/assets/img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atiki" src="../src/assets/img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atuc" src="../src/assets/img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atdort" src="../src/assets/img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atbes" src="../src/assets/img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atalti" src="../src/assets/img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atyedi" src="../src/assets/img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atsekiz" src="../src/assets/img/att.gif" width="50px" height="50px" />
  </div>
  <br />
  <br />
  <Button></Button>

</template>

<style scoped>
.included {
  margin-top: 10px;
  width: 100%;
  height: 100%;
  background-color: olivedrab;
}

.button {
  width: 90px;
  height: 60px;
  background-color:olivedrab;
  flex: content;
}
.finish {
  width: 10px;
  height: 558px;
  position: relative;
  float: right;
  background-color: black;
  margin-right: 10px;
}


</style>
