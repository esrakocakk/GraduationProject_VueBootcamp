<script setup>
import CountDownModal from '../Countdown/CountDownModal.vue';

function openModal() {
  this.isShowModal = true;
}
</script>

<template>

  <button class="button" @click="openModal()" >Yarışı Başlat</button> <!--Oyun başlangıcında geri sayım modalının da aktif eder-->
  <CountDownModal></CountDownModal>
</template>

<style>
.button {
  margin: 20px;
  margin-left: 300px;
  width: 220px;
  height: 65px;
  background-color: olivedrab;
  font-family: "Times New Roman", Times, serif;
  font-size: 20px;
}
</style>
