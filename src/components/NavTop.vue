<template>
    <div class="fixed right-0 w-full z-20">
      <div class="flex justify-between text-zinc-800  bg-zinc-200 h-16">
        <div v-show="LabelImage === false" class="bg-slate-800  mm:block pt-3.5 px-[0.76em] ">
          <img class="w-10" src="../assets/images/download.png" alt="logo">
        </div>
        <div v-show="LabelImage" class="hidden sm:block bg-slate-800 pt-4 md:pt-0 md:-mt-2 lg:block px-[1.12em] ">
          <img class="md:w-32 hidden lg:block md:py-8 md:mb-5 md:block md:mx-8 hidden" src="../assets/images/logo-light.a768f0d4.png" alt="logo">
          <img class="w-10  md:hidden" src="../assets/images/download.png" alt="logo">
        </div>
        <div class="flex relative flex-1 py-2">
          <i @click="conditionLabel" class="fa fa-bars pt-2 text-xl px-4 cursor-pointer" aria-hidden="true"></i>
          <div @click="CreateDrop = !CreateDrop " class="flex hidden md:block ml-4 cursor-pointer">
            <h4 class="mt-2">Create</h4>
            <i class="fa fa-angle-down relative -top-7 left-12 pt-3 ml-2" aria-hidden="true"></i>
          </div>
          <ul :class="CreateDrop ? 'block' : 'hidden'" class="translate-y-3 z-10 absolute transition-transform duration-200 left-16 top-16 bg-white rounded p-4">
            <li class="my-2">Action</li>
            <li class="my-2">Another action</li>
            <li class="my-2">Something Else here</li>
            <li class="my-2 mt-4">Separated link</li>
          </ul>
        </div>
        <div class="flex gap-3 py-2 relative">
          <i @click="SearchDrop = !SearchDrop" class="fa fa-search mr-2 text-lg pt-2 cursor-pointer" aria-hidden="true"></i>
          <div :class="SearchDrop ? 'block' : 'hidden'" class="bg-white translate-y-3 absolute top-16 sm:-left-28 -left-24 transition-transform duration-200 rounded p-4">
            <input id="search" class="bg-white border rounded p-0.5 border-gray-400 my-3">
            <label for="search" class="bg-blue-800 p-1 rounded relative -left-0.5">
              <i class="fa fa-search text-md mb-2 mx-2 text-white text-sm" aria-hidden="true"></i>
            </label>
          </div>
          <div class="xl:block hidden">
            <div @click="FlagDrop = !FlagDrop" class="flex py-3 cursor-pointer">
              <img  class="w-6 h-4 mr-2 mt-1" src="../assets/images/6.jpg" alt="flag">
              <span class="text-sm">English</span>
              <i class="fa fa-angle-down pt-0.5 ml-2" aria-hidden="true"></i>
            </div>
            <ul :class="FlagDrop ? 'block' : 'hidden'" class="grid gap-2 absolute transition-transform duration-200 top-20 bg-white left-12 rounded p-4 z-10">
              <li class="cursor-pointer flex my-2">
                <img class="w-6 h-4 mx-2 mt-1" src="../assets/images/2.jpg" alt="flag">
                <span class="text-sm">Spanish</span>
              </li>
              <li class="cursor-pointer flex my-2">
                <img class="w-6 h-4 mx-2 mt-1" src="../assets/images/3.jpg" alt="flag">
                <span class="text-sm">French</span>
              </li>
              <li class="cursor-pointer flex my-2">
                <img class="w-6 h-4 mx-2 mt-1" src="../assets/images/4.jpg" alt="flag">
                <span class="text-sm">Italian</span>
              </li>
              <li class="cursor-pointer flex my-2">
                <img class="w-6 h-4 mx-2 mt-1" src="../assets/images/5.jpg" alt="flag">
                <span class="text-sm">German</span>
              </li>
              <li class="cursor-pointer flex my-2">
                <img class="w-6 h-4 mx-2 mt-1" src="../assets/images/1.jpg" alt="flag">
                <span class="text-sm">Russian</span>
              </li>
            </ul>
          </div>
          <i class="fa fa-external-link text-xl mt-2.5 cursor-pointer" aria-hidden="true"></i>
          <div class="mx-3 relative">
            <i @click="BellDrop = !BellDrop" class="fa fa-bell-o text-lg pt-2 cursor-pointer" aria-hidden="true"></i>
            <div class="bg-red-600 top-2 left-3 absolute rounded-full h-4 w-4">
              <span class="text-white text-xs relative left-1 bottom-1.5">2</span>
            </div>
            <div :class="BellDrop ? 'block' : 'hidden'" class="w-[33vh] transition-all duration-200 text-slate-600 absolute bg-white z-10 -left-36 sm:-left-52 top-20 rounded">
              <h2 class="bg-white mb-5 text-center border-b relative py-2 font-bold">Notification(258)</h2>
              <div class="overflow-hidden bg-zinc-100 w-[33vh] h-[28vh] overflow-y-scroll">
                <div class="flex m-1 w-[33vh] hover:bg-slate-100 my-2 cursor-pointer">
                  <div class="w-28 h-14 mt-2 text-white bg-green-800 rounded-full">
                    <i class="fa fa-shopping-basket relative left-5 top-3.5" aria-hidden="true"></i>
                  </div>
                  <div class="ml-2">
                    <h4 class="font-bold text-ms">Your order is placed</h4>
                    <p class="text-xs font-bold text-slate-500">Dummy text of the printing and typesetting industry</p>
                  </div>
                </div>
                <div class="flex m-1 w-[33vh] hover:bg-slate-100 my-2 cursor-pointer">
                  <div class="w-28 h-14 text-white bg-blue-800 rounded-full">
                    <i class="fa fa-shopping-basket relative left-5 top-3.5" aria-hidden="true"></i>
                  </div>
                  <div class="ml-2">
                    <h4 class="font-bold text-ms">Your order is placed</h4>
                    <p class="text-xs font-bold text-slate-500">Dummy text of the printing and typesetting industry</p>
                  </div>
                </div>
                <div class="flex m-1 w-[33vh] hover:bg-slate-100 my-2 cursor-pointer">
                  <div class="w-28 h-14 text-white bg-red-500 rounded-full">
                    <i class="fa fa-shopping-basket relative left-5 top-3.5" aria-hidden="true"></i>
                  </div>
                  <div class="ml-2">
                    <h4 class="font-bold text-ms">Your order is placed</h4>
                    <p class="text-xs font-bold text-slate-500">Dummy text of the printing and typesetting industry</p>
                  </div>
                </div>
                <div class="flex m-1 w-[33vh] hover:bg-slate-100 my-2 cursor-pointer">
                  <div class="w-28 h-14 text-white bg-yellow-300 rounded-full">
                    <i class="fa fa-shopping-basket relative left-5 top-3.5" aria-hidden="true"></i>
                  </div>
                  <div class="ml-2 hover:bg-slate-100 my-2 cursor-pointer">
                    <h4 class="font-bold text-ms">Your order is placed</h4>
                    <p class="text-xs font-bold text-slate-500">Dummy text of the printing and typesetting industry</p>
                  </div>
                </div>
                <div class="flex m-1 w-[33vh] hover:bg-slate-100 my-2 cursor-pointer">
                  <div class="w-28 h-14 text-white bg-yellow-800 rounded-full">
                    <i class="fa fa-shopping-basket relative left-5 top-3.5" aria-hidden="true"></i>
                  </div>
                  <div class="ml-2">
                    <h4 class="font-bold text-ms">Your order is placed</h4>
                    <p class="text-xs font-bold text-slate-500">Dummy text of the printing and typesetting industry</p>
                  </div>
                </div>
              </div>
              <button class="text-center w-full border-t mt-3 hover:text-blue-500 font-bold mt-2">View all</button>
            </div>
          </div>
          <div class="relative">
            <img @click="ImageDrop = !ImageDrop" class="rounded-full mt-2 w-8 h-8 cursor-pointer" :class="{'showPopup': shownPopup ==='image'}" src="../assets/images/person1.jpg" alt="photo">
            <div :class="ImageDrop ? 'block':'hidden'" class="text-slate-600 z-10 transition-all duration-200  text-center bg-white absolute top-16 sm:-left-20 w-60 -left-48 sm:w-32">
              <div class="p-2 hover:bg-slate-100 hover:text-black cursor-pointer">
                <i class="fa fa-user-circle-o" aria-hidden="true"></i>
                <span class="ml-2">Profile</span>
              </div>
              <div class="p-2 hover:bg-slate-100 hover:text-black cursor-pointer">
                <i class="fa fa-briefcase" aria-hidden="true"></i>
                <span class="ml-2">Profile</span>
              </div>
              <div class="p-2 hover:bg-slate-100 hover:text-black cursor-pointer">
                <i class="fa fa-cog" aria-hidden="true"></i>
                <span class="ml-2">Profile</span>
              </div>
              <div class="p-2 hover:bg-slate-100 hover:text-black cursor-pointer">
                <i class="fa fa-unlock-alt" aria-hidden="true"></i>
                <span class="ml-2">Profile</span>
              </div>
              <div class="p-2 border-t hover:bg-slate-100 cursor-pointer">
                <span class="ml-2 text-red-500">Logout</span>
              </div>
            </div>
          </div>
          <div>
            <i @click="e" class="fa fa-cogs text-xl pt-2 pr-3 cursor-pointer" aria-hidden="true"></i>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
import SettingBar from '../components/SettingBar'

export default {
  data(){
    return{
      CreateDrop:false,
      SearchDrop:false,
      FlagDrop:false,
      BellDrop:false,
      ImageDrop:false,
      LabelImage:true,
    }
  },
  components:{
    SettingBar
  },
  methods:{
    condition(){
      this.show = !this.show
    },
    e(){
      this.$emit('setting')
    },
    conditionLabel(){
      this.LabelImage = !this.LabelImage
      this.$emit('nav')
    }
  },
}
</script>

