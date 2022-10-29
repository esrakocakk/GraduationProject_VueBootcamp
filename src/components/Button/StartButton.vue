<script setup>
import { ref } from "vue";
import CountDownModal from "../Countdown/CountDownModal.vue";

const isShowModal = ref(false);

function openModal() {
  this.isShowModal = true;
}
</script>

<template>
  <!--Oyun başlangıcında geri sayım modalının da aktif eder-->
  <button class="startButton" @click="openModal()">Yarışı Başlat</button>
  <CountDownModal v-if="isShowModal"></CountDownModal>
</template>

<style>
.startButton {
  margin-top: 45px;
  margin-left: 500px;
  width: 220px;
  height: 65px;

  font-family: "Times New Roman", Times, serif;
  font-size: 20px;
}
</style>
