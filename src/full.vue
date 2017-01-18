<template>
  <div :class="className" :style="style"></div>
</template>

<style scoped>
</style>

<script>
  import ECharts from 'echarts';
  // import Resize from 'element-resize-event';
  import Resize from 'element-resize-detector';
  import Wrapper from './wrapper.js';
  import world from './world.js';

  const IEcharts = Wrapper(ECharts, Resize, world);
  export default IEcharts;
</script>
