<script setup>
function startTimer(duration, display) {
  var timer = duration,
    minutes,
    seconds;
  setInterval(function () {
    seconds = parseInt(timer % 60, 10);
    seconds = seconds < 10 ? "0" + seconds : seconds;

    display.textContent = seconds;

    if (--timer < 0) {
      timer = duration;
    }
  }, 1000);
}

window.onload = function () {
  var fiveSeconds = 60 * 5,
    display = document.querySelector("#time");
  startTimer(fiveSeconds, display);
};
</script>

<template>
  <div class="time"><span id="time">5</span> Saniye!</div>
</template>

<style scoped>
.time {
  margin-top: 50px;
  text-align: center;
  font-size: 36px;
}
</style>
