<script setup>
import StartButton from "../Button/StartButton.vue";

const min = 20;
const max = 40;

const horsesData = [
  {
    id: "atbir",
    position: 5 + "px",
    image: "../img/att.gif",
  },
  {
    id: "atiki",
    position: 10 + "px",
    image: "../img/att.gif",
  },
  {
    id: "atuc",
    position: 15 + "px",
    image: "../img/att.gif",
  },
  {
    id: "atdort",
    position: 20 + "px",
    image: "../img/att.gif",
  },

  {
    id: "atbes",
    position: 25 + "px",
    image: "../img/att.gif",
  },
  {
    id: "atalti",
    position: 30 + "px",
    image: "../img/att.gif",
  },
  {
    id: "atyedi",
    position: 35 + "px",
    image: "../img/att.gif",
  },
  {
    id: "atsekiz",
    position: 40 + "px",
    image: "../img/att.gif",
  },
];

const horseData = horsesData[Math.floor(Math.random() * horsesData.length)];
console.log(horseData);

const timerId = setInterval(() => 1000);

function Start() {
  return;
}

function randomNumber() {
  speed = Math.floor(Math.random() * (max - min + 1)) + min;
  return;
}

console.log(horsesData);
</script>

<template>
  <div class="included">
    <div class="finish"></div>
    <div>
      <ul>
        {{horseData}}
      </ul>
    </div>
  </div>
  <center>
    <button class="button" v-on:click="Start()">Yarışı Başlat</button>
  </center>
</template>

<style scoped>
.included {
  margin-top: 10px;
  width: 100%;
  height: 100%;
  background-color: olivedrab;
}

.img {
  transition: all 2s;
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
