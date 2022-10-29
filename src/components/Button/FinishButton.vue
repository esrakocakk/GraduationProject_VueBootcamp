<script setup>
import { ref } from "vue";
import ResultModal from "../ResultTable/ResultModal.vue";

const isShowModal = ref(false);

function openModal() {
  this.isShowModal = true;
}
</script>

<template>
  <ResultModal v-if="isShowModal"></ResultModal>

  <!--Oyun başlangıcında geri sayım modalının da aktif eder-->
  <button class="finishButton" @click="openModal()">Sonuçları Göster</button>
</template>

<style>
.finishButton {
  float: right;

  margin-right: 10px;
  width: 60px;
  height: 30px;

  font-family: "Times New Roman", Times, serif;
  font-size: 12px;
}
</style>
