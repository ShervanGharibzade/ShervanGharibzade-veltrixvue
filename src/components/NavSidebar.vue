<template>
  <div class="fixed bg-slate-800 h-full z-10 mt-16 text-slate-500 xl:h-[100vh] overflow-y-scroll">
    <div class="px-5 relative top-24">
      <h4 class="uppercase text-xs mb-8">main</h4>
      <div class="flex transition my-2 p-2 cursor-pointer	duration-200 hover:text-slate-400">
        <p class="flex-1 text-lg">
          <i class="fa fa-home pt-1 w-7" aria-hidden="true"></i>
          <span>Dashboard</span>
        </p>
        <div class="bg-purple-600 w-6 h-6 rounded-full text-gray-300">
          <span class="relative left-2">2</span>
        </div>
      </div>
      <div class="flex transition my-2 p-2 cursor-pointer	duration-200 hover:text-slate-400">
        <p class="flex-1 text-lg">
          <i class="fa fa-calendar pt-1 w-7" aria-hidden="true"></i>
          <span>Calender</span>
        </p>
      </div>
      <div @click="conditionEmail" ref="EmailBack" class="flex z-10 cursor-pointer transition-all duration-500 my-2	 p-2 hover:text-slate-400">
        <p class="flex-1 text-lg">
          <i class="fa fa-envelope-o pt-1 w-7" aria-hidden="true"></i>
          <span>Email</span>
        </p>
        <i ref="email" class="fa fa-angle-down pt-2 mr-2 transition duration-200" aria-hidden="true"></i>
      </div>
      <ul ref="EmailInfo" class="ml-8 h-[0] transition-all duration-300">
        <li class="my-2 z-0 hover:text-slate-400">Inbox</li>
        <li class="my-2 z-0 hover:text-slate-400">Email Read</li>
        <li class="my-2 z-0 hover:text-slate-400">Email Compose</li>
      </ul>
      <div class="bg-slate-800 relative">
        <h4 class="uppercase text-xs py-8">components</h4>
        <div ref="UiInfo" class="relative bg-slate-800 transition-all duration-500">
          <div ref="UiBack" @click="conditionUi" class="flex py-2 p-2 cursor-pointer	 hover:text-slate-400">
            <p class="flex-1 text-lg">
              <i class="fa fa-archive pt-1 w-7" aria-hidden="true"></i>
              <span>UI Elements</span>
            </p>
            <i ref="ui" class="fa fa-angle-down pt-2 mr-2 transition duration-200" aria-hidden="true"></i>
          </div>
          <ul class="ml-8 h-[0] transition-all relative z-0 duration-300">
            <li class="my-2 z-0 hover:text-slate-400">item 1</li>
            <li class="my-2 z-0 hover:text-slate-400">item 2</li>
            <li class="my-2 z-0 hover:text-slate-400">item 3</li>
            <li class="my-2 z-0 hover:text-slate-400">item 4</li>
          </ul>
        </div>
        <div ref="FormtInfo" class="relative bg-slate-800 transition-all duration-500">
          <div @click="conditionForm" ref="FormBack" class="flex bg-slate-800 relative py-2 p-2 cursor-pointer hover:text-slate-400">
            <p class="flex-1 text-lg">
              <i class="fa fa-file-text pt-1 w-7" aria-hidden="true"></i>
              <span>Form</span>
            </p>
            <div class="bg-green-600 w-6 h-6 rounded-full text-gray-300">
              <span class="relative left-2">6</span>
            </div>
          </div>
          <ul class="ml-8 relative z-0 h-[0] transition-all duration-300">
            <li class="my-2 z-0 hover:text-slate-400">item 1</li>
            <li class="my-2 z-0 hover:text-slate-400">item 2</li>
            <li class="my-2 z-0 hover:text-slate-400">item 3</li>
            <li class="my-2 z-0 hover:text-slate-400">item 4</li>
          </ul>
        </div>
        <div ref="ChartInfo" class="relative bg-slate-800 transition-all duration-500">
          <div @click="conditionChart" ref="CharBack" class="flex bg-slate-800 relative py-2 p-2 cursor-pointer hover:text-slate-400">
            <p class="flex-1 text-lg">
              <i class="fa fa-pie-chart pt-1 w-7 " aria-hidden="true"></i>
              <span>Charts</span>
            </p>
            <i ref="chart" class="fa fa-angle-down pt-2 mr-2 transition duration-200" aria-hidden="true"></i>
          </div>
          <ul class="ml-8 h-[0] relative z-0 transition-all duration-300">
            <li class="my-2 z-0 hover:text-slate-400">item 1</li>
            <li class="my-2 z-0 hover:text-slate-400">item 2</li>
            <li class="my-2 z-0 hover:text-slate-400">item 3</li>
            <li class="my-2 z-0 hover:text-slate-400">item 4</li>
          </ul>
        </div>
        <div  ref="TableInfo" class="bg-slate-800 relative transition-all duration-500">
          <div @click="conditionTable" ref="TableBack" class="flex  bg-slate-800 relative py-2 p-2 cursor-pointer	 hover:text-slate-400">
            <p class="flex-1 text-lg">
              <i class="fa fa-table pt-1 w-7" aria-hidden="true"></i>
              <span>Tables</span>
            </p>
            <i ref="table" class="fa fa-angle-down pt-2 mr-2" aria-hidden="true"></i>
          </div>
          <ul class="ml-8 h-[0] b-slate-800 transition-all duration-300">
            <li class="my-2 z-0 hover:text-slate-400">item 1</li>
            <li class="my-2 z-0 hover:text-slate-400">item 2</li>
            <li class="my-2 z-0 hover:text-slate-400">item 3</li>
            <li class="my-2 z-0 hover:text-slate-400">item 4</li>
          </ul>
        </div>
        <div ref="IconInfo" class="bg-slate-800 relative transition-all duration-500">
          <div @click="conditionIcon" ref="IconBack" class="flex transition bg-slate-800 relative py-2 p-2 cursor-pointer	duration-200 hover:text-slate-400">
            <p class="flex-1 text-lg">
              <i class="fa fa-smile-o pt-1 w-7" aria-hidden="true"></i>
              <span>Icons</span>
            </p>
            <i ref="icon" class="fa fa-angle-down pt-2 mr-2" aria-hidden="true"></i>
          </div>
          <ul class="ml-8 h-[0] b-slate-800 transition-all duration-300">
            <li class="my-2 z-0 hover:text-slate-400">item 1</li>
            <li class="my-2 z-0 hover:text-slate-400">item 2</li>
            <li class="my-2 z-0 hover:text-slate-400">item 3</li>
            <li class="my-2 z-0 hover:text-slate-400">item 4</li>
          </ul>
        </div>
        <div ref="back" @click="conditionGoogle" class="flex transition bg-slate-800 relative py-2 p-2 cursor-pointer	duration-200 hover:text-slate-400">
          <p class="flex-1 text-lg">
            <i class="fa fa-map-marker pt-1 w-7" aria-hidden="true"></i>
            <span>Google Map</span>
          </p>
          <div class="bg-red-600 w-6 h-6 rounded-full text-gray-300">
            <span class="relative left-2">2</span>
          </div>
        </div>
      </div>
      <h4 class="uppercase bg-slate-800 relative text-xs py-8">Extras</h4>
      <div ref="AuthIfo" class="bg-slate-800 transition-all duration-500">
        <div ref="AuthBack" @click="conditionAuth" class="flex transition bg-slate-800 relative py-2 p-2 cursor-pointer duration-200 hover:text-slate-400">
          <p class="flex-1 text-lg">
            <i class="fa fa-stop pt-1 w-7" aria-hidden="true"></i>
            <span>Authentication</span>
          </p>
          <i ref="auth" class="fa fa-angle-down pt-2 mr-2" aria-hidden="true"></i>
        </div>
        <ul class="ml-8 h-[0] b-slate-800 transition-all duration-300">
          <li class="my-2 z-0 hover:text-slate-400">item 1</li>
          <li class="my-2 z-0 hover:text-slate-400">item 2</li>
          <li class="my-2 z-0 hover:text-slate-400">item 3</li>
          <li class="my-2 z-0 hover:text-slate-400">item 4</li>
        </ul>
      </div>
      <div ref="Pageinfo" class="bg-slate-800 relative transition-all duration-500 overflow-hidden">
        <div @click="conditionPage" ref="PageBack" class="flex transition bg-slate-800 relative py-2 p-2 cursor-pointer	duration-200 hover:text-slate-400">
          <p class="flex-1 text-lg">
            <i class="fa fa-suitcase pt-1 w-7" aria-hidden="true"></i>
            <span>Extra Pages</span>
          </p>
          <i ref="page" class="fa fa-angle-down pt-2 mr-2" aria-hidden="true"></i>
        </div>
        <ul class="ml-8 h-[0] b-slate-800 transition-all duration-300">
          <li class="my-2 z-0 hover:text-slate-400">item 1</li>
          <li class="my-2 z-0 hover:text-slate-400">item 2</li>
          <li class="my-2 z-0 hover:text-slate-400">item 3</li>
          <li class="my-2 z-0 hover:text-slate-400">item 4</li>
        </ul>
      </div>
      <div ref="TempInfo" class="bg-slate-800 relative transition-all duration-500 overflow-hidden">
        <div ref="TempBack" @click="conditionTemp" class="flex transition bg-slate-800 relative py-2 p-2 cursor-pointer	duration-200 hover:text-slate-400">
          <p class="flex-1 text-lg">
            <i class="fa fa-window-restore pt-1 w-7" aria-hidden="true"></i>
            <span>Extra Templates</span>
          </p>
          <i ref="temp" class="fa fa-angle-down pt-2 mr-2" aria-hidden="true"></i>
        </div>
        <ul class="ml-8 h-[0] b-slate-800 transition-all duration-300">
          <li class="my-2 z-0 hover:text-slate-400">item 1</li>
          <li class="my-2 z-0 hover:text-slate-400">item 2</li>
          <li class="my-2 z-0 hover:text-slate-400">item 3</li>
          <li class="my-2 z-0 hover:text-slate-400">item 4</li>
        </ul>
      </div>
      <div ref="MultiInfo" class="bg-slate-800 relative transition-all duration-500 overflow-hidden">
        <div @click="conditionMulti" ref="MultiBack" class="flex transition bg-slate-800 relative py-2 p-2 cursor-pointer	duration-200 hover:text-slate-400">
          <p class="flex-1 text-lg">
            <i class="fa fa-ellipsis-h pt-1 w-7" aria-hidden="true"></i>
            <span>Multi level</span>
          </p>
          <i ref="mulit" class="fa fa-angle-down pt-2 mr-2" aria-hidden="true"></i>
        </div>
        <ul class="ml-8 h-[0] b-slate-800 transition-all duration-300">
          <li class="my-2 z-0 hover:text-slate-400">item 1</li>
          <li class="my-2 z-0 hover:text-slate-400">item 2</li>
          <li class="my-2 z-0 hover:text-slate-400">item 3</li>
          <li class="my-2 z-0 hover:text-slate-400">item 4</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  data(){
    return{
      remot:false
    }
  },
  props:['change'],
  methods:{
    conditionEmail(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.email.classList.add('rotate-180')
        this.$refs.EmailBack.classList.add('bg-slate-700')
        this.$refs.EmailInfo.classList.add('h-[100px]')
        this.$refs.EmailInfo.classList.remove('h-[0]')
      }
      else{
        this.$refs.email.classList.remove('rotate-180')
        this.$refs.EmailBack.classList.remove('bg-slate-700')
        this.$refs.EmailInfo.classList.remove('h-[100px]')
        this.$refs.EmailInfo.classList.add('h-[0]')
      }
    },
    conditionUi(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.ui.classList.add('rotate-180')
        this.$refs.UiBack.classList.add('bg-slate-700')
        this.$refs.UiInfo.classList.add('h-[180px]')
        this.$refs.UiInfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.ui.classList.remove('rotate-180')
        this.$refs.UiBack.classList.remove('bg-slate-700')
        this.$refs.UiInfo.classList.remove('h-[180px]')
        this.$refs.UiInfo.classList.add('h-[35px]')
      }
    },
    conditionForm(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.FormBack.classList.add('bg-slate-700')
        this.$refs.FormtInfo.classList.add('h-[180px]')
        this.$refs.FormtInfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.FormBack.classList.remove('bg-slate-700')
        this.$refs.FormtInfo.classList.remove('h-[180px]')
        this.$refs.FormtInfo.classList.add('h-[35px]')
      }
    },
    conditionChart(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.chart.classList.add('rotate-180')
        this.$refs.CharBack.classList.add('bg-slate-700')
        this.$refs.ChartInfo.classList.add('h-[180px]')
        this.$refs.ChartInfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.chart.classList.remove('rotate-180')
        this.$refs.CharBack.classList.remove('bg-slate-700')
        this.$refs.ChartInfo.classList.remove('h-[180px]')
        this.$refs.ChartInfo.classList.add('h-[35px]')
      }
    },
    conditionTable(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.table.classList.add('rotate-180')
        this.$refs.TableBack.classList.add('bg-slate-700')
        this.$refs.TableInfo.classList.add('h-[180px]')
        this.$refs.TableInfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.table.classList.remove('rotate-180')
        this.$refs.TableBack.classList.remove('bg-slate-700')
        this.$refs.TableInfo.classList.remove('h-[180px]')
        this.$refs.TableInfo.classList.add('h-[35px]')
      }
    },
    conditionIcon(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.icon.classList.add('rotate-180')
        this.$refs.IconBack.classList.add('bg-slate-700')
        this.$refs.IconInfo.classList.add('h-[180px]')
        this.$refs.IconInfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.icon.classList.remove('rotate-180')
        this.$refs.IconBack.classList.remove('bg-slate-700')
        this.$refs.IconInfo.classList.remove('h-[180px]')
        this.$refs.IconInfo.classList.add('h-[35px]')
      }
    },
    conditionGoogle(){
      this.remot = !this.remot
      if (this.remot)
        this.$refs.back.classList.add('bg-slate-700')
      else
        this.$refs.back.classList.remove('bg-slate-700')
    },
    conditionAuth(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.AuthBack.classList.add('bg-slate-700')
        this.$refs.AuthIfo.classList.add('h-[180px]')
        this.$refs.AuthIfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.AuthBack.classList.remove('bg-slate-700')
        this.$refs.AuthIfo.classList.remove('h-[180px]')
        this.$refs.AuthIfo.classList.add('h-[35px]')
      }
    },
    conditionPage(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.PageBack.classList.add('bg-slate-700')
        this.$refs.Pageinfo.classList.add('h-[180px]')
        this.$refs.Pageinfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.PageBack.classList.remove('bg-slate-700')
        this.$refs.Pageinfo.classList.remove('h-[180px]')
        this.$refs.Pageinfo.classList.add('h-[35px]')
      }
    },
    conditionTemp(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.TempBack.classList.add('bg-slate-700')
        this.$refs.TempInfo.classList.add('h-[180px]')
        this.$refs.TempInfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.TempBack.classList.remove('bg-slate-700')
        this.$refs.TempInfo.classList.remove('h-[180px]')
        this.$refs.TempInfo.classList.add('h-[35px]')
      }
    },
    conditionMulti(){
      this.remot = !this.remot
      if (this.remot){
        this.$refs.MultiBack.classList.add('bg-slate-700')
        this.$refs.MultiInfo.classList.add('h-[180px]')
        this.$refs.MultiInfo.classList.remove('h-[35px]')
      }
      else{
        this.$refs.MultiBack.classList.remove('bg-slate-700')
        this.$refs.MultiInfo.classList.remove('h-[180px]')
        this.$refs.MultiInfo.classList.add('h-[35px]')
      }
    }
  },
  computed:{
    changeHeight(){
      if(this.change)
        this.$refs.nav.classList.add('h-10')
    }
  }
}
</script>
