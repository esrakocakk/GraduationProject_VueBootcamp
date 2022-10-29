<script setup>
import Horses from "./components/Horses/Horses.vue";
import Leaderboard from "./components/ResultTable/Leaderboard.vue";
import CountDownModal from "./components/Countdown/CountDownModal.vue"
import ResultTable from "./components/ResultTable/ResultTable.vue"
import ResultModal from "./components/ResultTable/ResultModal.vue";
</script>

<template>
  <Horses></Horses>
    <Leaderboard></Leaderboard>
  <CountDownModal></CountDownModal>
  <ResultModal></ResultModal>
</template>

<style >

</style>
