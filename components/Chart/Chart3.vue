<template>
  <div class="chart-3">
    <canvas id="my-chart-3"></canvas>
  </div>
</template>

<script setup lang="ts">
import Chart from "chart.js/auto";

const labels = ["Jan", "Feb", "Mar", "Apr", "Mei", "Jun", "Jul"];
const number_1 = [30, 20, 67, 22, 45, 59, 24];
const number_2 = [20, 40, 77, 12, 65, 89, 94];

const data = {
  labels: labels,
  datasets: [
    {
      label: "Dataset 1",
      data: number_1,
      borderColor: "rgb(255, 99, 132)",
      backgroundColor: "rgb(255, 99, 132)",
      stack: "combined",
      type: "bar",
    },
    {
      label: "Dataset 2",
      data: number_2,
      borderColor: "rgb(54, 162, 235)",
      backgroundColor: "rgb(54, 162, 235)",
      stack: "combined",
    },
  ],
};

const config = {
  type: "line",
  data: data,
  options: {
    plugins: {
      title: {
        display: true,
        text: "Chart.js Stacked Line/Bar Chart",
      },
    },
    scales: {
      y: {
        stacked: true,
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
  const myChart = document.getElementById("my-chart-3") as any;
  myChart.height = 240;
  myChart.width = 400;
  new Chart(myChart, config as any);
});
</script>

<style>
.chart-3 {
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
