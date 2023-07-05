<template>
  <div class="app p-10">
    <h1 class="font-bold text-xl m-5">Bar</h1>
    <ChartComponent />
    <h1 class="font-bold text-xl m-5">Line</h1>
    <ChartLine />
    <h1 class="font-bold text-xl m-5">Radar</h1>
    <ChartRadar />
    <h1 class="font-bold text-xl m-5">Doughnut</h1>
    <ChartDoughnut />
    <h1 class="font-bold text-xl m-5">Doughnut</h1>
    <ChartPie />
    <h1 class="font-bold text-xl m-5">Bubble</h1>
    <ChartBubble />
  </div>
</template>

<script>
import ChartComponent from "@/components/ChartComponent.vue";
import ChartLine from "@/components/ChartLine.vue";
import ChartRadar from "@/components/ChartRadar.vue";
import ChartDoughnut from "@/components/ChartDoughnut.vue";
import ChartPie from "@/components/ChartPie.vue";
import ChartBubble from "@/components/ChartBubble.vue";
export default {
  components: {
    ChartComponent,
    ChartLine,
    ChartRadar,
    ChartDoughnut,
    ChartPie,
    ChartBubble,
  },
};
</script>
