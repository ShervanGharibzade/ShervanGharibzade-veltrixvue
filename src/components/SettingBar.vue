<template>
  <div @click.self="e" class="fixed z-50 top-0 right-0 w-full bg-zinc-600/30">
    <div class="bg-white text-black relative z-50 float-right px-6 h-[100vh] top-0 right-0 w-72 overflow-hidden overflow-y-scroll">
      <h2 class="my-6">Setting</h2>
      <i @click="e" class="fa fa-times absolute cursor-pointer text-xl top-6 right-7" aria-hidden="true"></i>
      <div>
        <div>
          <h4 class="border-b mb-5">Layout</h4>
          <div>
            <label for="toggle" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Horizontal
              </div>
            </label>
          </div>
          <div class="flex items-center my-2 w-full">
            <label for="toggle2" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle2" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Vertical
              </div>
            </label>
          </div>
        </div>
        <div>
          <h4 class="border-b my-5">Width</h4>
          <div>
            <label for="toggle8" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle8" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Fluid
              </div>
            </label>
          </div>
          <div class="flex items-center my-2 w-full">
            <label for="toggle7" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle7" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Boxed
              </div>
            </label>
          </div>
        </div>
        <div>
          <h4 class="border-b my-5">Sidebar</h4>
          <div>
            <label for="toggle3" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle3" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Dark
              </div>
            </label>
          </div>
          <div class="flex items-center my-2 w-full">
            <label for="toggle4" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle4" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Light
              </div>
            </label>
          </div>
          <div class="flex items-center my-2 w-full">
            <label for="toggle5" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle5" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Compact
              </div>
            </label>
          </div>
          <div class="flex items-center my-2 w-full">
            <label for="toggle6" class="flex items-center cursor-pointer">
              <div class="relative">
                <input type="checkbox" id="toggle6" class="sr-only">
                <div class="block bg-white border-gray-400 border w-8 h-4 rounded-full"></div>
                <div class="dot absolute bg-gray-400 left-1 top-0.5 bg-white w-3 h-3 rounded-full transition"></div>
              </div>
              <div class="ml-3 text-sm">
                Icon
              </div>
            </label>
          </div>
        </div>
        <div>
          <h4 class="border-t pt-2 text-center my-5">Choose Layouts</h4>
          <div class="grid grid-cols-1 gap-5">
            <img class="border-4 p-1 rounded" src="../assets/images/b1.jpg" alt="pic">
            <img class="border-4 p-1 rounded" src="../assets/images/b2.jpg" alt="pic">
            <img class="border-4 p-1 rounded" src="../assets/images/b3.jpg" alt="pic">
            <button class="bg-purple-600 hover:bg-purple-800 transition duration-200 dur mx-auto px-6 py-3 m-1 rounded text-white">
              <i class="fa fa-shopping-basket" aria-hidden="true"></i>
              <span class="ml-2">Purchase Now</span>
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{

    }
  },
  methods:{
    e(){
      this.$emit('close')
    }
  },
}
</script>
