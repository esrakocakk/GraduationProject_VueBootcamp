<script setup>
import Horses from "./components/Horses/Horses.vue";
import StartButton from "./components/Button/StartButton.vue";
import AgainButton from "./components/Button/AgainButton.vue";
</script>

<template>
  <div class="included">
    <div class="finish" id="finish"></div>
    <Horses></Horses>
  </div>
  <br />
  <br />
  <StartButton></StartButton>

  <AgainButton></AgainButton>
</template>

<style scoped>
.included {
  margin-top: 10px;
  width: 100%;
  height: 100%;
  background-color: olivedrab;
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
