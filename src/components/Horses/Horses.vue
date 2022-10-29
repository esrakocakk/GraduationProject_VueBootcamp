<script setup>
import FinishButton from '../Button/FinishButton.vue';
const min = 20;
const max = 40;

//atların random seçilmesi için oluşturulan data
const horsesData = [
  {
    id: "atbir",
    position: 5 + "px",
  },
  {
    id: "atiki",
    position: 10 + "px",
  },
  {
    id: "atuc",
    position: 15 + "px",
  },
  {
    id: "atdort",
    position: 20 + "px",
  },
  {
    id: "atbes",
    position: 25 + "px",
  },
  {
    id: "atalti",
    position: 30 + "px",
  },
  {
    id: "atyedi",
    position: 35 + "px",
  },
  {
    id: "atsekiz",
    position: 40 + "px",
  },
];

//ile atlardan bir tanesi random olarak seçilmekte
const horseData = horsesData[Math.floor(Math.random() * horsesData.length)];

function horse() {}

console.log(horseData);

function Start() {
  setInterval(horseData, 1000);
  return;
}

// position fonksiyonu ile atların hızları 20 ile 40 sayıalrı arasından bir değer alacak şekilde belirleniyor
function position() {
  speed = Math.floor(Math.random() * (max - min + 1)) + min;
  return;
}
</script>

<template>
  <div class="included">
    <div class="finish"></div>

    <!--Horse Datadan gelen random atlar vfor aracılığıyla ekrana yansıtılıyor ve hareket işlemleri gerçekleşiyor -->
    <img
      class="image"
      v-for="horseData in horsesData"
      src="../img/att.gif"
      :class="`margin-left:${horsesData.position}px`"
    />
    <FinishButton></FinishButton>
  </div>
  
</template>

<style scoped>
.included {
  margin-top: 10px;
  width: 100%;
  height: 550px;
  background-color: olivedrab;
}

.image {
  margin: 10px;
  display: flex;
  width: 60px;
  height: 60px;
  transition: all 2s;
}
.start {
  position: fixed;
  margin: 0;
  margin-left: 80px;
  width: 10px;
  height: 550px;
  position: relative;
  float: left;
  background-color: black;
}
.finish {
  position: fixed;
  width: 10px;
  height: 550px;
  position: relative;
  float: right;
  background-color: black;
  margin-right: 10px;
}
</style>
