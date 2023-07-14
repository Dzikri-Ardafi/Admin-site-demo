<template>
  <div class="chart-2">
    <canvas id="my-chart-2"></canvas>
  </div>
</template>

<script setup lang="ts">
import Chart from "chart.js/auto";

const datas = [63, 123, 233, 244, 78, 111, 35];
const CHART_COLORS = {
  red: "rgb(255, 99, 132)",
  orange: "rgb(255, 159, 64)",
  yellow: "rgb(255, 205, 86)",
  green: "rgb(75, 192, 192)",
  blue: "rgb(54, 162, 235)",
  purple: "rgb(153, 102, 255)",
  grey: "rgb(201, 203, 207)",
};

const data = {
  labels: ["Red", "Orange", "Yellow", "Green", "Blue"],
  datasets: [
    {
      label: "Dataset 1",
      data: datas,
      backgroundColor: Object.values(CHART_COLORS),
    },
  ],
};

const config = {
  type: "pie",
  data: data,
  options: {
    responsive: true,
    plugins: {
      legend: {
        position: "top",
      },
      title: {
        display: true,
        text: "Pie Chart",
      },
    },
  },
};
onMounted(() => {
  const myChart = document.getElementById("my-chart-2") as any;
  myChart.height = 200;
  new Chart(myChart, config as any);
});
</script>

<style>
.chart-2 {
  border-radius: 20px;
  background: linear-gradient(
    313deg,
    #fbfbfb55 0%,
    rgba(178, 204, 255, 0.267) 80.64%
  );
  box-shadow: 3px 3px 50px 0px rgba(0, 0, 0, 0.25);
  padding: 0.5em;
}
</style>
