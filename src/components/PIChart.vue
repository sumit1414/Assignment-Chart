<template>
  <div>
    <div class="mx-auto">
      <GChart type="PieChart" class="w-full" :options="options" :data="data" />
    </div>
  </div>
</template>

<script>
import { GChart } from "vue-google-charts";
export default {
  name: "App",
  components: {
    GChart,
  },
  data() {
    return {
      data: [
        ["Daily Routine", "Hours per Day"],
        ["Tasks are Closed", 3],
        ["Task are Inprogress", 1],
        ["Task are New", 4],
      ],
      options: {
        height: 400,
      },
    };
  },
};
</script>
