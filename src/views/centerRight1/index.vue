<template>
  <div class="centerRight1">
    <div class="bg-color-black">
      <div class="d-flex pt-2 pl-2">
        <span>
          <i class="iconfont icon-chart-line" />
        </span>
        <div class="d-flex">
          <span class="fs-xl text mx-2 mt-1">模型性能</span>
        </div>
      </div>
      <div>
        <chart />
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import Chart from "./chart/index";
export default defineComponent({
  components: {
    Chart
  }
})
</script>

<style lang="scss" scoped>
$box-height: 410px;
$box-width: 400px;
.centerRight1 {
  padding: 20px 16px;
  height: $box-height;
  width: $box-width;
  border-radius: 5px;
  .bg-color-black {
    height: $box-height - 35px;
    border-radius: 10px;
  }
  .text {
    color: #c3cbde;
  }
  .chart-box {
    margin-top: 16px;
    width: 170px;
    height: 170px;
    .active-ring-name {
      padding-top: 10px;
    }
  }
}
</style>
