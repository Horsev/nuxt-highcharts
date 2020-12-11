<template lang="pug">
section
  h1 Hello Highcharts
  highcharts(:options="chartOptions")
</template>

<script>
export default {
  data () {
    return {
      chartOptions: {
        xAxis: {
          type: 'datetime'
        },
        series: [{
          data: [1, 2, 3]
        }],
        plotOptions: {
          series: {
            pointIntervalUnit: 'month',
            pointInterval: 1
          }
        }
      }
    }
  }
}
</script>
