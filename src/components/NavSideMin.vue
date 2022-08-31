<template>
  <div class="bg-slate-800 w-16 text-slate-500 h-full">
    <div class="grid grid-cols-1 z-10 py-4 pb-32 justify-center text-center">
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-home mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute z-10 left-20 top-[4.8em] hidden group-hover:block text-slate-300">
          <li class="p-[1.12em] bg-slate-700">Dashboard</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-calendar mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute left-20 top-[8.6em] hidden group-hover:block text-slate-300">
          <li class="p-[1.11em] bg-slate-700">Calender</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-envelope-o mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[8.5em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.12em] pr-20 bg-slate-700">Emali</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Inbox</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-archive mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[12.3em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.11em] pr-20 bg-slate-700 w-52">UI Elements</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item3</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item4</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item5</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item6</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item7</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-file-text mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[16em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.12em] pr-20 bg-slate-700">Forms</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item3</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item4</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-pie-chart mx-auto text-2xl pt-1 w-7 " aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[19.8em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.11em] pr-20 bg-slate-700">Charts</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item3</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item4</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-table pt-1 mx-auto text-2xl w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[23.5em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.12em] pr-20 bg-slate-700">Tables</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-smile-o pt-1 mx-auto text-2xl w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[27.3em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.11em] pr-20 bg-slate-700">Tables</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-map-marker mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[31em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.12em] pr-20 bg-slate-700">Tables</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-stop mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[34.8em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.11em] pr-20 bg-slate-700">Tables</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-suitcase mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[38.5em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.12em] pr-20 bg-slate-700">Tables</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-window-restore mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[42.3em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.11em] pr-20 bg-slate-700">Tables</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
        </ul>
      </div>
      <div class="hover:bg-slate-700 cursor-pointer py-3 group">
        <i class="fa fa-ellipsis-h mx-auto text-2xl pt-1 w-7" aria-hidden="true"></i>
        <ul class="bg-slate-800 absolute text-start z-10 left-16 top-[46em] hidden group-hover:block text-slate-300">
          <li class="pl-3 py-[1.12em] pr-20 bg-slate-700">Tables</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item1</li>
          <li class="pl-5 py-5 pr-20 bg-slate-800 hover:text-slate-100">Item2</li>
        </ul>
      </div>
    </div>
  </div>
</template>
