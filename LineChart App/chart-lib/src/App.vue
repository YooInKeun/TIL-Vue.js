<template>
  <div id="app">
    <h1>Chart.js</h1>
    <bar-chart></bar-chart>
    <line-chart></line-chart>
  </div>
</template>

<script>
import BarChart from './components/BarChart.vue';
import LineChart from './components/LineChart.vue';

export default {
  components: {
    BarChart,
    LineChart,
  },
  data() {
    return {
    }
  },
  methods: {
  },
  created() {
  }
}
</script>

<style>

</style>
