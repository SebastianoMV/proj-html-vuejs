<template>
  <div class="flex-wrapper">
  
  
  <div class="single-chart">
    <svg viewBox="0 0 36 36" class="circular-chart green">
      <path class="circle-bg"
        d="M18 2.0845
          a 15.9155 15.9155 0 0 1 0 31.831
          a 15.9155 15.9155 0 0 1 0 -31.831"
      />
      <path class="circle" :stroke-dasharray="`${ratePercent}, 100`" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"
      />
      <text x="18" y="20.35" class="percentage">{{ratePercent}}%</text>
    </svg>
  </div>

</div>
</template>

<script>
export default {
  name: 'RateComp',
  props:{
    ratePercent: Number,
  }

}
</script>

<style lang="scss" scoped>
@import '../assets/style/var';

.flex-wrapper {
  display: flex;
  justify-content: center;
}

.single-chart {
  width: 100%;
  justify-content: center ;
}

.circular-chart {
  display: block;
  margin: 10px auto;
  max-width: 80%;
  max-height: 250px;
}

.circle-bg {
  fill: none;
  stroke: #eee;
  stroke-width: 2;
}

.circle {
  fill: none;
  stroke-width: 2;
  stroke-linecap: round;
  animation: progress 1s ease-out forwards;
}

@keyframes progress {
  0% {
    stroke-dasharray: 0 100;
  }
}

.circular-chart.green .circle {
  stroke: $primary-color;
}


.percentage {
  fill: #8d959f;
  font-family: sans-serif;
  font-size: 0.5em;
  text-anchor: middle;
}

</style>