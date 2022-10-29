<script setup>
import Horses from '../Horses/Horses.vue';
</script>
<template>
<table class="Leader-table" border="2">
    <tr>
      <th>Liderlik Tablosu</th>
    </tr>
    <tr>
      <th>Önde Gelen At: {{}}</th> <!--Horses Vue dosyasından gelen verilere göre slotla promplanmış bilgi burada yanstılıyor-->
    </tr>
  </table>
</template>
<style scoped>
.Leader-table {
  margin: -68px;
  width: 220px;
  height: 68px;
  margin-left: 800px;
  border: 3px solid olive;
  text-align: center;
}
</style>