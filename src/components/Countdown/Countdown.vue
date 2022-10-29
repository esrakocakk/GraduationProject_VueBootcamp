<script setup>
function startTimer(duration, display) {
  var timer = duration,
    seconds;
  setInterval(function () {
    seconds = parseInt(timer % 10, 10);

    seconds = seconds < 10 ? "0" + seconds : seconds;

    display.textContent = seconds;

    if (--timer < 0) {
      timer = duration;
    }
  }, 1000);
}

window.onload = function () {
  var tenSecond = 60 * 5,
    display = document.querySelector("#time");
  startTimer(tenSecond, display);
};
</script>

<template>
  <div class="time"><span id="time">10</span><br> Saniye!</div>
</template>

<style scoped>
.time {
  margin-top: 50px;
  text-align: center;
  font-size: 36px;
}
</style>
