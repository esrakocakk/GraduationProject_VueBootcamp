<script setup>
import { ref } from 'vue';
import Countdown from '../Countdown/Countdown.vue';

const showModal=ref(false);

</script>

<template>
  <Countdown></Countdown>
  <center>
    <button @click="showModal = true">show</button>
    <button class="button" @click="showModal=true">Yarışı Başlat</button>
  </center>
</template>

<style>
.button {
  margin: 20px;
  width: 150px;
  height: 55px;
  font-family: "Times New Roman", Times, serif;
  font-size: 20px;
  background-color: olivedrab;
}
</style>
