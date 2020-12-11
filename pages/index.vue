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
        series: [
          {
            data: [1, 2, 3]
          }
        ]
      }
    }
  }
}
</script>
