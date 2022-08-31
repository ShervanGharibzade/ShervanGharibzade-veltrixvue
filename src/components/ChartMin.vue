<template>
  <div class="w-full lg:w-1/3 relative h-full bg-white p-4">
    <h2 class="text-black py-2">Sales Analytics</h2>
    <div class="grid w-3/4 md:w-full pt-3 md:flex border-b justify-start md:justify-center">
      <div class="text-black grid">
        <p>Online</p>
        <p class="font-bold">1,542</p>
      </div>
      <div id="chart">
        <apexchart type="line" height="100" :options="chartOptions" :series="series"></apexchart>
      </div>
    </div>
    <div class="md:flex pt-3 w-3/4 md:w-full grid border-b justify-start md:justify-center">
      <div class="text-black grid">
        <p>offline</p>
        <p class="font-bold">6,451</p>
      </div>
      <div id="chart2">
        <apexchart type="line" height="100" :options="chartOptions" :series="series"></apexchart>
      </div>
    </div>
    <div class="md:flex pt-3 w-3/4 md:w-full grid justify-start md:justify-center">
      <div class="text-black grid">
        <p>marketing</p>
        <p class="font-bold">84,574</p>
      </div>
      <div id="chart3">
        <apexchart type="line" height="100" :options="chartOptions" :series="series"></apexchart>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      series: [
        {
          name: "High - 2013",
          data: [1,10,3,17,4,10]
        }
      ],
      chartOptions: {
        chart: {
          height: 350,
          type: 'line',
          dropShadow: {
            enabled: false,
            color: '#000',
            top: 18,
            left: 7,
            blur: 10,
            opacity: 0.2
          },
          toolbar: {
            show: false
          }
        },
        colors: ['#77B6EA', '#545454'],
        dataLabels: {
          enabled: false,
        },
        stroke: {
          curve: 'straight',
        },
        fill:{
          type: 'solid',
          opacity:[1,0.35]
        },
        grid: {
          borderColor: '#e7e7e7',
          row: {
            colors: ['#f3f3f3', 'transparent'], // takes an array which will be repeated on columns
            opacity: 0.5
          },
        },
        markers: {
          size: 1
        },
        xaxis:{
          type:'numeric',
        },
        yaxis: {
          min: 0,
          max: 20
        },
        legend: {
          position: 'top',
          horizontalAlign: 'right',
          floating: true,
          offsetY: -25,
          offsetX: -5
        }
      },
    }
  }
}

</script>
