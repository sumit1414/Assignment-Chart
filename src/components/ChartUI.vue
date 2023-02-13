<template>
  <div class="grid grid-cols-2 gap-12 p-8">
    <div class="shadow-lg bg-white p-6 rounded-lg">
      <p class="text-left cursor-pointer">
        <span class="material-symbols-outlined fsize16"> edit_square </span>
        Meeting Notes:
        <span class="text-blue">...Read more</span>
      </p>

      <div class="flex justify-between mt-6 border-b pb-4">
        <div class="flex items-center">
          <p class="text-gray fsize14 flex items-center">
            <span class="material-symbols-outlined fsize17 mr-1"> history </span
            >Approved Estimate
          </p>
          <p class="text-white chips">19Hrs</p>
        </div>

        <div class="flex items-center">
          <p class="text-gray fsize14 flex items-center">
            <span class="material-symbols-outlined fsize17 mr-1"> timer </span
            >Total Time:
          </p>
          <p class="text-white chips-success">50Hrs</p>
        </div>
      </div>

      <div class="flex justify-between items-center mt-8 border-b pb-4">
        <div>
          <h2 class="text-success fsize30 { font-semibold text-success">30%</h2>
          <progress id="file" class="progcolor" value="32" max="100">
            32%
          </progress>
        </div>

        <div>
          <P class="text-gray">Productive Hours</P>
          <h4 class="text-black flex items-center justify-center font-semibold">
            <span class="material-symbols-outlined mr-1 fsize18 text-success">
              trending_up </span
            >47 Hrs
          </h4>
        </div>

        <div>
          <P class="text-gray">Learning Hours</P>
          <h4 class="text-danger font-semibold">+2 Hrs</h4>
        </div>
      </div>

      <PIChart />
    </div>
    <div class="shadow-lg bg-white p-6 rounded-lg">
      <p class="text-left cursor-pointer">
        <span class="material-symbols-outlined fsize16"> edit_square </span>
        Meeting Notes:
        <span class="text-blue">...Read more</span>
      </p>

      <div class="flex justify-between mt-6 border-b pb-4">
        <div class="flex items-center">
          <p class="text-gray fsize14 flex items-center">
            <span class="material-symbols-outlined fsize17 mr-1"> history </span
            >Approved Estimate
          </p>
          <p class="text-white chips">525Hrs</p>
        </div>

        <div class="flex items-center">
          <p class="text-gray fsize14 flex items-center">
            <span class="material-symbols-outlined fsize17 mr-1"> timer </span
            >Total Time:
          </p>
          <p class="text-white chips-success">120Hrs</p>
        </div>
      </div>

      <div class="flex justify-between items-center mt-8 border-b pb-4">
        <div>
          <h2 class="text-success fsize30 { font-semibold text-success">0%</h2>
          <progress id="file" class="progcolor grall" value="32" max="100">
            0%
          </progress>
        </div>

        <div>
          <P class="text-gray">Productive Hours</P>
          <h4 class="text-black flex items-center justify-center font-semibold">
            <span class="material-symbols-outlined mr-1 fsize18 text-success">
              trending_up </span
            >47 Hrs
          </h4>
        </div>

        <div>
          <P class="text-gray">Learning Hours</P>
          <h4 class="text-danger font-semibold">+120 Hrs</h4>
        </div>
      </div>

      <PIChart2 />
    </div>
  </div>
</template>

<script>
import PIChart from "./PIChart";
import PIChart2 from "./PIChart2";

export default {
  components: {
    PIChart,
    PIChart2,
  },
};
</script>

<style scoped>
.chips {
  background: #dc3545;
  font-size: 12px;
  padding: 3px 11px;
  border-radius: 12px;
  margin-left: 10px;
}
.progcolor {
  color: #75d375f7;
}
.chips-success {
  background: #75d375f7;
  font-size: 12px;
  padding: 3px 11px;
  border-radius: 12px;
  margin-left: 10px;
}
.fsize20 {
  font-size: 20px;
}
.fsize16 {
  font-size: 16px;
}
.progcolor {
  height: 8px;
}
.fsize18 {
  font-size: 18px;
}
.text-success {
  color: #75d375f7 !important;
}
.text-gray {
  color: gray;
}
.text-blue {
  color: blue;
}
.fsize30 {
  font-size: 30px;
}
.fsize14 {
  font-size: 14px;
}
progress {
  border: none;

  height: 60px;
  background: crimson;
  border-radius: 10px;
}

progress {
  color: lightblue;
}
.grall::-webkit-progress-bar {
  background: #f4f5f6 !important;
}
.grall::-webkit-progress-value {
  background: #f4f5f6 !important;
}
.grall::-webkit-progress-value {
  background: #75d375f7;
}
progress::-moz-progress-bar {
  background: lightblue;
}

progress::-webkit-progress-value {
  background: #75d375f7;
}

progress::-webkit-progress-bar {
  background: #f4f5f6;
}
.text-danger {
  color: #dc3545;
}
.bg-danger {
  background: "#dc3545";
}
</style>
