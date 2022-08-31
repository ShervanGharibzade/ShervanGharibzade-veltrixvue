<template>
  <div class="text-black bg-white p-4 m-2 overflow-hidden lg:overflow-x-hidden overflow-x-scroll">
    <h2 class="font-bold">Latest Trasaction</h2>
    <div class="w-[48em] xl:w-full lg:w-full">
      <div class="grid grid-cols-6 border-b border-b-2 pb-2">
        <span>(#) Id</span>
        <span>Name</span>
        <span>Date</span>
        <span>Amount</span>
        <span>Status</span>
      </div>
      <div class="grid my-2 p-1 hover:bg-blue-100/30 cursor-pointer grid-cols-6">
        <span>#14256</span>
        <div class="flex">
          <img class="w-8 rounded-full" src="../assets/images/person5.jpg" alt="pic">
          <span class="text-sm ml-1 mt-1">philip Smead</span>
        </div>
        <span>15/1/2018</span>
        <span>$94</span>
        <span class="text-sm bg-green-600 w-16 h-5 rounded text-white">Delivered</span>
        <button class="bg-blue-600 hover:bg-blue-800 rounded w-10 mx-auto text-white">Edit</button>
      </div>
      <div class="grid p-1 hover:bg-blue-100/30 cursor-pointer my-2 grid-cols-6">
        <span>#14257</span>
        <div class="flex">
          <img class="w-8 rounded-full" src="../assets/images/person4.jpg" alt="pic">
          <span class="text-sm ml-1 mt-1"> Brent Shipley</span>
        </div>
        <span>16/1/2019</span>
        <span>$112</span>
        <span class="text-sm bg-yellow-500 w-16 h-5 rounded text-white">Pendding</span>
        <button class="bg-blue-600 hover:bg-blue-800 rounded w-10 mx-auto text-white">Edit</button>
      </div>
      <div class="grid p-1 hover:bg-blue-100/30 cursor-pointer my-2 grid-cols-6">
        <span>#14258</span>
        <div class="flex">
          <img class="w-8 rounded-full" src="../assets/images/person3.jpg" alt="pic">
          <span class="text-sm ml-1 mt-1"> Robert Sitton</span>
        </div>
        <span>17/1/2019</span>
        <span>$116</span>
        <span class="text-sm bg-green-600 w-16 h-5 rounded text-white">Delivered</span>
        <button class="bg-blue-600 hover:bg-blue-800 rounded w-10 mx-auto text-white">Edit</button>
      </div>
      <div class="grid p-1 hover:bg-blue-100/30 cursor-pointer my-2 grid-cols-6">
        <span>#14259</span>
        <div class="flex">
          <img class="w-8 h-8 rounded-full" src="../assets/images/person2.jpg" alt="pic">
          <span class="text-sm ml-1 mt-1">Alberto Jac</span>
        </div>
        <span>18/1/2019</span>
        <span>$109</span>
        <span class="text-sm bg-red-500 w-12 h-5 rounded text-white">Cancle</span>
        <button class="bg-blue-600 hover:bg-blue-800 rounded w-10 mx-auto text-white">Edit</button>
      </div>
      <div class="grid p-1 hover:bg-blue-100/30 cursor-pointer my-2 grid-cols-6">
        <span>#14260</span>
        <div class="flex">
          <img class="w-8 h-8 rounded-full" src="../assets/images/person1.jpg" alt="pic">
          <span class="text-sm ml-1 mt-1">David Sanchez</span>
        </div>
        <span>15/1/2018</span>
        <span>$94</span>
        <span class="text-sm bg-green-600 w-16 h-5 rounded text-white">Delivered</span>
        <button class="bg-blue-600 hover:bg-blue-800 rounded w-10 mx-auto text-white h-8">Edit</button>
      </div>
      <div class="grid p-1 hover:bg-blue-100/30 cursor-pointer my-2 grid-cols-6">
        <span>#14261</span>
        <div class="flex">
          <img class="w-8 rounded-full" src="../assets/images/person5.jpg" alt="pic">
          <span class="text-sm ml-1 mt-1">philip Smead</span>
        </div>
        <span>15/1/2018</span>
        <span>$94</span>
        <span class="text-sm bg-yellow-500 w-16 h-5 rounded text-white">Pendding</span>
        <button class="bg-blue-600 hover:bg-blue-800 rounded w-10 mx-auto text-white">Edit</button>
      </div>
    </div>
  </div>
</template>
