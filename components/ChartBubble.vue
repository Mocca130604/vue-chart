<template>
  <div>
    <canvas ref="chartCanvas"></canvas>
  </div>
</template>

<script>
import Chart from "chart.js/auto";

export default {
  mounted() {
    this.renderChart();
  },
  methods: {
    renderChart() {
      const ctx = this.$refs.chartCanvas.getContext("2d");
      new Chart(ctx, {
        type: "bubble",
        data: {
          datasets: [
            {
              label: "Data",
              data: [
                { x: 10, y: 10, r: 10 },
                { x: 11, y: 20, r: 10 },
                { x: 12, y: 30, r: 10 },
                { x: 13, y: 40, r: 10 },
                { x: 14, y: 50, r: 10 },
                { x: 15, y: 10, r: 20 },
                { x: 50, y: 20, r: 15 },
                // tambahkan data bubble lainnya
              ],
              backgroundColor: "rgba(75, 192, 192, 0.6)",
              borderColor: "rgba(75, 192, 192, 1)",
            },
          ],
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          scales: {
            y: {
              beginAtZero: true,
            },
          },
        },
      });
    },
  },
};
</script>
