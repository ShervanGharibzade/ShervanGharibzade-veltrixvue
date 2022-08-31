<template>
  <div class="bg-blue-700 rounded m-2">
    <div class="p-5 relative">
      <div class="flex">
        <div class="bg-blue-200 h-14 rounded">
          <i :class="icon" class=" mt-2 px-3 text-2xl" aria-hidden="true"></i>
        </div>
        <div class="ml-6">
          <span class="uppercase text-zinc-300">{{ title }}</span>
          <p class="text-zinc-100 text-xl">
            {{ price }}
            <i class="fa fa-arrow-up text-green-500" aria-hidden="true"></i>
          </p>
        </div>
      </div>
      <div :class="color" class="absolute right-0 top-4">
        <span class="text-white px-3">
          {{ num }}
        </span>
      </div>
    <div class="flex text-blue-300 w-full mt-7">
      <p class="flex-1">Since last month</p>
      <i class="fa fa-arrow-right ml-3 mt-1.5" aria-hidden="true"></i>
    </div>
  </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      pop:'fa fa-address-book'
    }
  },
  // props:{
  //   title:{
  //     required: true,
  //     default: '',
  //     type: String,
  //   }
  // },
  props:['title' , 'icon' , 'color' , 'price' , 'num' ]
}
</script>
