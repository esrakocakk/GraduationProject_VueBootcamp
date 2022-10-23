<script setup>
import StartButton from "../Button/StartButton.vue";

</script>

<template>
  <div class="included">
   
    <div class="finish" id="finish"></div>
    
    <img id="atbir" src="../img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atiki" src="../img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atuc" src="../img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atdort" src="../img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atbes" src="../img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atalti" src="../img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atyedi" src="../img/att.gif" width="50px" height="50px" />
    <hr />
    <img id="atsekiz" src="../img/att.gif" width="50px" height="50px" />
    
  </div>
  <StartButton ></StartButton>
</template>

<style scoped>
.included {
  margin-top: 10px;
  width: 100%;
  height: 100%;
  background-color: olivedrab;
}
.start {
 margin: 0;
  margin-left: 80px;
  width: 10px;
  height: 558px;
  position: relative;
  float: left;
  background-color: black;
  
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
