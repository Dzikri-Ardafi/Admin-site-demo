<template>
  <div class="chart-1">
    <canvas id="my-chart"></canvas>
  </div>
</template>

<script setup lang="ts">
import Chart from "chart.js/auto";

const labels = [40, 30, 20];

const data = {
  labels: labels,

  datasets: [
    {
      axis: "y",
      label: "LOREM IPSUM",
      data: [65, 59],
      fill: false,
      backgroundColor: ["#D8B1FF", "#D8B1FF"],
      borderWidth: 1,
    },
    {
      axis: "y",
      label: "Amet Lorem",
      data: [25, 80, 30],
      fill: false,
      backgroundColor: ["#FFDB5C", "#FFDB5C", "#FFDB5C"],
      borderWidth: 1,
    },
  ],
};
const config = {
  type: "bar",
  data,
  options: {
    indexAxis: "y",
    scales: {
      y: {
        border: {
          width: 3,
        },
        grid: {
          lineWidth: 2,
        },

        ticks: {
          font: {
            weight: "bold",
          },
          color: "black",
        },
      },
      x: {
        border: {
          width: 3,
        },
        grid: {
          lineWidth: 2,
        },
        ticks: {
          font: {
            weight: "bold",
          },
          color: "black",
        },
      },
    },
  },
};

onMounted(() => {
  const myChart = document.getElementById("my-chart") as any;
  myChart.height = 200;
  new Chart(myChart, config as any);
});
</script>

<style>
.chart-1 {
  border-radius: 20px;
  background: linear-gradient(
    313deg,
    #fbfbfb 0%,
    rgba(178, 204, 255, 0.75) 80.64%
  );
  box-shadow: 3px 3px 20px 0px rgba(0, 0, 0, 0.25);
  padding: 0.5em;
}
</style>
