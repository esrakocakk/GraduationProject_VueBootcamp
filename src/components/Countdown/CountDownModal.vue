<script setup>
import Countdown from "./Countdown.vue";

const isShowModal = false;


</script>

<template>

  <div class="modal-mask" v-if="isShowModal">
    <div class="modal-container">
      <div class="modal-wrapper">
        <button class="modal-button">X</button>
        <div class="modal-header">Oyunun Başlamasına</div>
        <div class="modal-body">
          <Countdown></Countdown>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.modal-container {
  float: center;
  margin: 200px;
  margin-left: 600px;
  width: 300px;
  height: 200px;
  padding: 20px 30px;
  background-color: rgb(255, 255, 255);
  border-radius: 6px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.33);
  transition: all 0.3s ease;
  font-family: Helvetica, Arial, sans-serif;
}
.modal-mask {
  position: fixed;
  z-index: 9998;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: table;
  transition: opacity 0.3s ease;
}

.modal-wrapper {
  display: table-cell;
  vertical-align: middle;
}

.modal-header {
  margin-top: 10px;
  color: #0c0c0c;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 28px;
  font-style: normal;
  text-align: center;
}

.modal-body {
  margin: 20px 0;
}

.modal-button {
  margin: -10px;
  margin-left: 300px;
  float: right;
  width: 20px;
  height: 20px;
  background-color: rgb(250, 243, 243);
  border: 0px;
  text-align: center;
  font-size: 14px;
  font-family: Arial, Helvetica, sans-serif;
  font-style: inherit;
}
</style>
