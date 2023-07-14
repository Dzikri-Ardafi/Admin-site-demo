<template>
  <div class="chart-4">
    <canvas id="my-chart-4"></canvas>
  </div>
</template>

<script setup lang="ts">
import Chart from "chart.js/auto";

const labels = ["Jan", "Feb", "Mar", "Apr", "Mei", "Jun", "Jul"];
const datas = [65, 59, 80, 81, 56, 55, 40];
const bgColor = [
  "rgba(255, 99, 132, 0.2)",
  "rgba(255, 159, 64, 0.2)",
  "rgba(255, 205, 86, 0.2)",
  "rgba(75, 192, 192, 0.2)",
  "rgba(54, 162, 235, 0.2)",
  "rgba(153, 102, 255, 0.2)",
  "rgba(201, 203, 207, 0.2)",
];

const borderColor = [
  "rgb(255, 99, 132)",
  "rgb(255, 159, 64)",
  "rgb(255, 205, 86)",
  "rgb(75, 192, 192)",
  "rgb(54, 162, 235)",
  "rgb(153, 102, 255)",
  "rgb(201, 203, 207)",
];

const data = {
  labels: labels,
  datasets: [
    {
      label: "Dataset 1",
      data: datas,
      borderColor: "rgba(255, 255, 255, 0.703)",
      backgroundColor: "rgba(255, 143, 30, 0.584)",
      stack: "combined",
      type: "bar",
    },
  ],
};
const config = {
  type: "bar",
  data: data,
  options: {
    scales: {
      y: {
        beginAtZero: true,
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
  const myChart = document.getElementById("my-chart-4") as any;
  myChart.height = 215;
  new Chart(myChart, config as any);
});
</script>

<style>
.chart-4 {
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
