<script setup>
import StartButton from "../Button/StartButton.vue";


const min = 20;
const max = 40;

const horsesData = [
  {
    id: "atbir",
    position: 5 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
  {
    id: "atiki",
    position: 10 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
  {
    id: "atuc",
    position: 15 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
  {
    id: "atdort",
    position: 20 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
  {
    id: "atbes",
    position: 25 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
  {
    id: "atalti",
    position: 30 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
  {
    id: "atyedi",
    position: 35 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
  {
    id: "atsekiz",
    position: 40 + "px",
    image: {
      url: "../img/att.gif",
    },
  },
];

const horseData = horsesData[Math.floor(Math.random() * horsesData.length)];

function horse() {

}

console.log(horseData);

function Start() {
  setInterval(horseData, 1000);
  return;
}

function position() {
  speed = Math.floor(Math.random() * (max - min + 1)) + min;
  return;
}

console.log(horsesData);
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
  </div>
  <StartButton ></StartButton>
  
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
