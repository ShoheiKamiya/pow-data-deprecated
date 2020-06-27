<script>
import { Bar } from 'vue-chartjs'

export default {
  extends: Bar,
  data: () => ({
    datacollection: {
      labels: ['20', '21', '22'],
      datasets: [
        {
          label: 'Data One',
          backgroundColor: '#74b9ff',
          data: [40, 20, 30],
        },
      ],
    },
    options: {
      responsive: true,
      maintainAspectRatio: false,
    },
  }),

  mounted() {
    this.renderChart(this.datacollection, this.options)
  },
}
</script>
