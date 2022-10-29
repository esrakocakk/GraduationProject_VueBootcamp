<script setup>
import ResultTable from "./ResultTable.vue"
</script>

<template>
  <div class="modal-mask">
    <div class="modal-container">
      <div class="modal-wrapper">
        <button class="modal-button" @click="close">X</button>
        <div class="modal-body">
          <ResultTable></ResultTable>
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

.modal-body {
  margin: 0px ;
}

.modal-button {
  margin: 10px;
  margin-left: 10px;
  float: right;
  width: 20px;
  height: 20px;
  background-color:rgb(250, 243, 243);
  border: 0px;
  text-align: center;
  font-size: 14px;
  font-family: Arial, Helvetica, sans-serif;
  font-style:inherit
  }
</style>
