<template>
  <div class="w-full grid lg:w-full xl:w-full pr-10 md:pr-0 lg:flex bg-white p-4 mr-4 h-full">
    <div id="chart" class="w-full h-full lg:w-2/3">
      <h2 class="text-black">Monthly Earning</h2>
      <apexchart type="line" height="400" :options="chartOptions" :series="series"></apexchart>
    </div>
    <div class="h-2/4 lg:h-full lg:flex">
      <div class="w-full md:w-1/3 mx-auto grid gap-5 h-full text-black mt-10 text-center">
        <p >This month</p>
        <p class="font-bold pt-5">$34,252</p>
        <p>It will be as simple as in fact it will be occidental.</p>
        <div class="flex relative h-40 justify-center mt-10 justify-items-center">
          <div class="radial-progress text-zinc-300 absolute rounded" style="--value:100; --size:6em; --thickness: 10px;"></div>
          <div class="radial-progress hover:text-blue-400 cursor-pointer text-blue-500 absolute rounded" style="--value:75; --size:6em; --thickness: 10px;"></div>
        </div>
      </div>
      <div class="w-full md:w-1/3 mx-auto grid gap-5 h-2/4 lg:h-full mt-10 text-black text-center">
        <p>Last month</p>
        <p class="font-bold pt-5">$36,253</p>
        <p>It will be as simple as in fact it will be occidental.</p>
        <div class="flex relative h-40 mt-10 justify-center">
          <div class="radial-progress text-zinc-300 absolute rounded" style="--value:100; --size:6em; --thickness: 10px;"></div>
          <div class="radial-progress hover:text-blue-400 cursor-pointer text-blue-500 absolute rounded" style="--value:60; --size:6em; --thickness: 10px;"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data(){
      return{
        series: [{
          type: 'area',
          data: [5,9,7,8,5,3,5,4]
        }],
        chartOptions: {
          chart: {
            height: '500px',
            type: 'line',
          },
          stroke: {
            curve: 'smooth'
          },
          fill: {
            type:'solid',
            opacity: [0.35, 1],
          },
          labels: [1,2,3,4,5,6,7,8,9],
          markers: {
            size: 5
          },
          yaxis: {
            min: 1,
            max: 9
          },
          legend: {
            position: 'top',
            horizontalAlign: 'right',
            floating: true,
            offsetY: -25,
            offsetX: -5
          }
        },
          tooltip: {
            shared: true,
            intersect: false,
            y: {
              formatter: function (y) {
                if(typeof y !== "undefined") {
                  return  y.toFixed(0) + " points";
                }
                return y;
              }
            }
          }
        }
      }
    }

</script>
