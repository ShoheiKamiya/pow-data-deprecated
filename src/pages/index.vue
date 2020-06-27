<template>
  <div class="test">
    <snow-fall-chart :style="chartStyle" />
  </div>
</template>

<script>
import SnowFallChart from '@/components/SnowFallChart'
export default {
  components: {
    SnowFallChart,
  },
  computed: {
    chartStyle() {
      return {
        position: 'relative',
        height: '100%',
        width: '100%',
      }
    },
  },
}
</script>

<style>
.test {
  margin: 0 auto;
  width: 50%;
}
</style>
