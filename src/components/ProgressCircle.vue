<template>
  <div class="relative w-full m-2 h-full p-4 bg-white p-2 rounded">
    <h2 class="text-black mb-5">Sales Report</h2>
    <p class="text-black mb-5">
      <i class="fa fa-calendar-o text-blue-500" aria-hidden="true"></i>
      jan01 - jan31
      <span class="float-right mr-5 lg:mr-0 font-bold">
        $4230
      </span>
    </p>
    <div class="relative flex justify-center block h-60">
      <div class="radial-progress text-yellow-500 absolute  rounded" style="--value:100; --size:12em; --thickness: 10px;"></div>
      <div class="radial-progress text-green-500 absolute  rounded" style="--value:85; --size:12em; --thickness: 10px;"></div>
      <div class="radial-progress text-blue-500 absolute top-0 rounded" style="--value:55; --size:12em; --thickness: 10px;"></div>
    </div>
    <div>
      <p class="text-black grid grid-cols-3 gap-12 pb-2 border-b">
        <span class="bg-blue-500 w-12 text-white rounded p-1">Desk</span>
        <span class="mt-1">Desktop</span>
        <span class="mt-1">54.5%</span>
      </p>
      <p class="text-black grid grid-cols-3 gap-12 pb-2 border-b">
        <span class="bg-green-500 w-11 text-white rounded p-1">Mob</span>
        <span class="mt-1">Mobile</span>
        <span class="mt-1">28.0%</span>
      </p>
      <p class="text-black grid grid-cols-3 gap-12 pb-2 border-b">
        <span class="bg-yellow-500 w-8 text-white rounded p-1">Tab</span>
        <span class="mt-1">tablets</span>
        <span class="mt-1">17.5%</span>
      </p>
    </div>
  </div>
</template>
